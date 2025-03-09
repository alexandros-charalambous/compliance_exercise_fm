<template>
  <footer class="content">
    <div class="footer">
      <div class="logo-group">
        <img class="logo1" src="@/assets/logo.svg" alt="Logo1" />
        <img class="logo2" src="@/assets/logo2.svg" alt="Logo2" />
      </div>
      <div class="section">
        <div class="footer-text">
          <p>
            Finance Magnates Intelligence, part of Finance Magnates, delivers
            specialized research and insights on the financial markets. Offering
            Quarterly, Annual, and custom reports tailored to specific business
            needs, it covers key aspects such as trading volumes, market trends,
            regulations, and more
          </p>
          <div class="socialmedia">
            <img src="@/assets/twitter.svg" />
            <img src="@/assets/telegram.svg" />
            <img src="@/assets/youtube.svg" />
            <img src="@/assets/facebook.svg" />
            <img src="@/assets/linkedin.svg" />
            <img src="@/assets/rss.svg" />
          </div>
        </div>
        <div class="menu">
          <ul>
            <li>Finance Magnates</li>
            <li>Latest News</li>
            <li>Directory</li>
            <li>Events</li>
            <li>Contact Us</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="copyright">
      <p>© 2024 "Finance Magnates CY Ltd." All rights reserved.</p>
      <div class="policies">
        <ul>
          <li>Cookie Policy</li>
          <li>Privacy Policy</li>
          <li>Terms and Conditions</li>
          <li>Manage Cookies</li>
        </ul>
      </div>
    </div>
  </footer>
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
    padding: 64px;
    gap: 32px;
  }

  @media (max-width: 767px) {
    padding: 64px 16px;
    gap: 34px;
  }
}

.footer {
  display: flex;
  flex-direction: row;
  gap: 48px;

  @media (max-width: 1439px) {
    flex-direction: column;
  }

  @media (max-width: 767px) {
  }
}

.logo-group {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  top: 8px;

  @media (max-width: 1439px) {
    flex-direction: row;
    padding-top: 8px;
    padding-right: 20px;
  }

  @media (max-width: 767px) {
    height: 165.84px;
    flex-direction: column;
  }
}

.logo1 {
  width: 195px;
  top: 0.8px;
}

.logo2 {
  width: 172px;
}

.section {
  display: flex;
  flex-direction: row;
  gap: 48px;

  @media (max-width: 767px) {
    flex-direction: column;
  }
}

.footer-text {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  min-width: 288px;
  gap: 24px;
}

.footer-text p {
  color: var(--color-text-secondary);
  font-weight: 400;
  font-size: 18px;
  line-height: 28px;
}

.socialmedia {
  display: flex;
  gap: 18px;
}

.menu {
  display: flex;
  color: var(--color-text-secondary);
  height: 166px;
  min-width: 215px;
  padding-left: 24px;
  padding-right: 24px;
  gap: 8px;

  @media (max-width: 767px) {
    padding: 0px;
  }
}

.menu ul {
  display: grid;
  padding: 0;
  list-style-type: none;
}

.menu ul li {
  font-weight: 400;
  font-size: 18px;
  line-height: 28px;
}

.copyright {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  color: var(--color-text-secondary);
  gap: 12px;

  @media (max-width: 1439px) {
    flex-direction: column;
  }
}

.copyright p {
  font-weight: 400;
  font-size: 14px;
  line-height: 22px;
}

.policies ul {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  list-style-type: none;
  column-gap: 24px;
  padding: 0px;
  text-decoration: underline;
  font-weight: 500;
  font-size: 12px;
  line-height: 20px;
}
</style>
