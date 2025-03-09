<template>
  <section class="content">
    <div class="section-h">
      <h1>Frequently Asked Questions</h1>
    </div>
    <div class="section-p">
      <div>
        <h1>How often is the Compliance Industry Report available?</h1>
        <p>
          The report is published monthly, providing regular updates to help
          businesses stay ahead of compliance changes.
        </p>
      </div>
      <div>
        <h1>How can I access the Monthly Compliance Industry Report?</h1>
        <p>
          Simply fill out the form on this page to get the report delivered
          straight to your inbox.
        </p>
      </div>
      <div>
        <h1>How is the data in the report gathered?</h1>
        <p>
          The report uses trusted sources like global regulators, industry news,
          expert analysis, and input from compliance professionals.
        </p>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.content {
  display: flex;
  flex-direction: column;
  height: 100%;
  padding: 96px 64px;
  background-color: var(--color-background-primary);
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

.section-h {
  width: auto;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.section-h h1 {
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

.section-p {
  display: flex;
  flex-wrap: wrap;
  gap: 64px;
  @media (max-width: 767px) {
    gap: 24px;
  }
}

.section-p div {
  display: flex;
  flex-direction: column;
  width: 100%;
  min-width: 150px;
  gap: 8px;
  flex: 1 1 calc(33.333% - 64px);

  @media (max-width: 1439px) {
    flex: 1 1 calc(50% - 64px);
  }

  @media (max-width: 767px) {
    gap: 24px;
    flex: 1 1 100%;
  }
}

.section-p h1 {
  color: var(--color-text-primary);
  font-weight: 400;
  font-size: 18px;
  line-height: 28px;

  @media (max-width: 767px) {
    font-weight: 600;
    font-size: 18px;
  }
}

.section-p p {
  color: var(--color-text-secondary);
  font-weight: 400;
  font-size: 18px;
  line-height: 28px;

  @media (max-width: 767px) {
    font-size: 16px;
    line-height: 24px;
  }
}
</style>
