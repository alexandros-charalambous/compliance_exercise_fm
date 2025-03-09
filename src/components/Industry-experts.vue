<template>
  <section class="content">
    <div class="title">
      <h1>Prepared by industry experts</h1>
      <p>Meet our Team behind our intelligence insights.</p>
    </div>
    <div class="cards">
      <div v-for="(card, index) in cards" :key="index" class="card">
        <img :src="card.image" :alt="card.alt" />
        <div class="card-p">
          <h1>{{ card.title }}</h1>
          <p>{{ card.description }}</p>
        </div>
      </div>
    </div>
    <div class="dots">
      <span
        v-for="(_, index) in cards"
        :key="index"
        class="dot"
        :class="{ active: index === currentIndex }"
        @click="moveSlide(index)"
      ></span>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";

const cards = ref([
  {
    image: new URL("@/assets/card1.png", import.meta.url).href,
    alt: "Card1",
    title: "Sylwester Majewski",
    description:
      "A graduate of the Warsaw School of Economics, Sylwester received an MA specializing in finance and banking. As Finance Magnates’ research associate and STA certified analyst, he leaves no stone unturned. Sylwester is the previous minority partner of an NFA registered US forex broker, and since 2003, has participated in many forex projects.",
  },
  {
    image: new URL("@/assets/card2.png", import.meta.url).href,
    alt: "Card2",
    title: "Ramzi Ahmad",
    description:
      "With over 16 years of experience in data-driven marketing within the financial industry, Ramzi Ahmad has developed expertise across Fintech, Crypto, Payments, and Online Trading markets. He has led teams to improve efficiency and drive growth for dozens of financial brands through actionable data insights. Ramzi continues to advance his skills through courses at institutions like Harvard and Cambridge, ensuring the highest standards of data accuracy.",
  },
  {
    image: new URL("@/assets/card3.png", import.meta.url).href,
    alt: "Card3",
    title: "Damian Chmiel",
    description:
      "Damian’s adventure with the financial markets began at the Cracow University of Economics, where obtained his MA in finance and accounting. Starting from the retail trader perspective, he collaborated with brokerage houses and financial portals in Poland as an independent editor and content manager. His adventure in Finance Magnates began in 2016 where he develops as a business intelligence analyst.",
  },
]);

const currentIndex = ref(0);

const moveSlide = (index) => {
  const cardContainer = document.querySelector(".cards");
  const cardWidth = document.querySelector(".card").offsetWidth;
  const gap = 30;

  cardContainer.scrollTo({
    left: index * (cardWidth + gap),
    behavior: "smooth",
  });
  currentIndex.value = index;
};
</script>

<style scoped>
.content {
  display: flex;
  flex-direction: column;
  height: 100%;
  padding: 96px 64px;
  background-color: var(--color-background-secondary);
  gap: 64px;

  @media (max-width: 1439px) {
    gap: 32px;
    padding: 64px;
  }

  @media (max-width: 767px) {
    gap: 24px;
    padding: 32px 16px;
  }
}

.title {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.title h1 {
  color: var(--color-text-primary);
  font-weight: 600;
  font-size: 36px;
  line-height: 44px;

  @media (max-width: 767px) {
    font-weight: 600;
    font-size: 24px;
    line-height: 32px;
  }
}

.title p {
  color: var(--color-text-secondary);
  font-weight: 400;
  font-size: 20px;
  line-height: 30px;
}

.cards {
  overflow-x: scroll;
  display: flex;
  flex-direction: row;
  height: 100%;
  gap: 30px;
  scrollbar-width: none;
}

.card {
  display: flex;
  flex-direction: column;
  width: 378px;
  padding: 32px;
  border-radius: 16px;
  background: var(--color-background-primary);

  position: relative;

  @media (max-width: 767px) {
    width: 255px;
    padding: 22px;
  }
}

.card::before {
  content: "";
  pointer-events: none;
  position: absolute;
  inset: 0;
  padding: 1px;
  border-radius: inherit;
  background: linear-gradient(180deg, #ffffff4d, #ffffff00);
  mask: linear-gradient(white 0 0) content-box, linear-gradient(white 0 0);
  background-clip: xor;
  mask-composite: exclude;
}

.card img {
  height: 300px;
  width: 314px;
  border-radius: 8px;

  @media (max-width: 767px) {
    height: 214px;
    width: 214px;
  }
}

.card-p {
  display: flex;
  flex-direction: column;
  padding-top: 24px;
  gap: 16px;
}

.card-p h1 {
  color: var(--color-text-primary);
  font-weight: 600;
  font-size: 24px;
  line-height: 32px;
}

.card-p p {
  color: var(--color-text-secondary);
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
}

.dots {
  display: flex;
  gap: 21px;
  justify-content: center;
}

.dot {
  height: 8px;
  width: 8px;
  background-color: #808080;
  border-radius: 50%;
  cursor: pointer;
}
.dot.active {
  background-color: white;
  height: 10px;
  width: 10px;
}
</style>
