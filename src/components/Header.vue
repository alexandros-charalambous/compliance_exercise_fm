<template>
  <header>
    <div class="logo">
      <img src="@/assets/logo.svg" alt="Logo" />
    </div>

    <div class="vector1">
      <img src="@/assets/Vector1.svg" alt="Vector1" />
    </div>
    <div class="vector2">
      <img src="@/assets/Vector2.svg" alt="Vector2" />
    </div>

    <div class="content">
      <div class="content-article">
        <h1>Stay Informed. Stay Compliant.</h1>
        <p>
          Sign up to access the latest Insights on Regulatory Highlights, Recent
          Developments, and Future Outlook—all in one monthly report.
        </p>
      </div>
      <div class="content-box">
        <h1>Get your free compliance guide</h1>
        <form class="content-form">
          <div class="form-fields">
            <div class="field">
              <label>First name</label>
              <input type="text" placeholder="John" />
            </div>
            <div class="field">
              <label>Last name</label>
              <input type="text" placeholder="Doe" />
            </div>
            <div class="field">
              <label>Email Address</label>
              <input type="text" placeholder="you@company.com" />
            </div>
            <div class="field">
              <label>Company</label>
              <input type="text" placeholder="Enter company name" />
            </div>
          </div>
          <div class="submit">
            <button type="button" @click="submit">Get Free Report</button>
            <div class="terms">
              <p class="terms-p1">
                By submitting this form, you agree to our
                <span class="underline-p1">Privacy Policy</span>.
              </p>
              <p class="terms-p2">
                This site is protected by reCAPTCHA and the Google Privacy
                Policy and
                <span class="underline-p2">Terms of Service</span>
                apply.
              </p>
            </div>
          </div>
        </form>
      </div>
    </div>
  </header>
</template>

<script setup>
const submit = () => {};
</script>

<style scoped>
header {
  width: 100%;
  position: relative;
  padding: 27px 64px 64px 64px;
  display: flex;
  justify-content: space-between;
  gap: 96px;
  flex-direction: column;

  @media (max-width: 1439px) and (min-width: 768px) {
    gap: 54px;
  }

  @media (max-width: 767px) {
    padding: 32px 16px;
    gap: 24px;
  }
}

.vector1 {
  overflow-x: hidden;
  position: absolute;
  z-index: -1;
  top: 0px;
  right: 0px;
}

.vector2 {
  overflow-x: hidden;
  position: absolute;
  z-index: -1;
  right: 0px;
  bottom: 0px;
}

.logo {
  display: flex;
  align-items: center;
  height: 46px;

  img {
    height: auto;
  }
}

.content {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  gap: 100px;

  @media (max-width: 1439px) {
    flex-direction: column;
    gap: 54px;
  }
}

.content-article {
  width: auto;
  color: var(--color-text-primary);
  display: flex;
  flex-direction: column;
  gap: 36px;
}

.content-article h1 {
  font-weight: 700;
  font-size: 60px;

  @media (max-width: 1439px) {
    font-weight: 600;
    font-size: 48px;
  }

  @media (max-width: 767px) {
    font-weight: 600;
    font-size: 30px;
  }
}

.content-article p {
  font-weight: 400;
  font-size: 20px;

  @media (max-width: 767px) {
    font-size: 16px;
  }
}

.content-box {
  width: 576px;
  min-width: 576px;
  display: flex;
  flex-direction: column;
  border: 1px solid #acaeb7;
  border-radius: 16px;
  padding: 48px;
  gap: 48px;
  background-color: var(--color-background-secondary);

  @media (max-width: 767px) {
    width: 100%;
    max-width: 576px;
    min-width: 0px;
    padding: 32px;
  }
}

.content-box h1 {
  color: var(--color-text-primary);
  font-weight: 600;
  font-size: 24px;
}

.content-form {
  display: flex;
  flex-direction: column;
  gap: 32px;
  color: var(--color-text-secondary);
}

.form-fields {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.field div label {
  font-weight: 500;
  font-size: 16px;
}

.field input {
  width: 100%;
  height: 44px;
  color: var(--color-text-primary);
  border: 1px solid var(--color-border);
  border-radius: 4px;
  padding: 10px 14px;
  background-color: var(--color-background-secondary);
}

.submit {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.submit button {
  width: 100%;
  padding: 12px 32px;
  color: var(--color-text-primary);
  background-color: var(--color-alt);
  border: 0px;
  border-radius: 4px;
  font-weight: 600;
  font-size: 16px;
}

.terms {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.terms-p1 {
  font-weight: 400;
  font-size: 16px;
}

.underline-p1 {
  color: var(--color-text-primary);
  text-decoration: underline;
}

.terms-p2 {
  font-weight: 400;
  font-size: 14px;
}

.underline-p2 {
  text-decoration: underline;
}
</style>
