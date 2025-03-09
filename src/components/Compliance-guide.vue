<template>
  <section class="content">
    <div class="section-h">
      <h1>Your Monthly Compliance Guide</h1>
      <p>
        The Finance Magnates Compliance Industry Report provides an overview of
        key regulatory changes to help businesses navigate compliance challenges
      </p>
    </div>
    <div class="section-p">
      <div>
        <h1>Regulatory Updates</h1>
        <p>
          Explore the latest changes from major regulators so you can adjust
          your operations confidently.
        </p>
      </div>
      <div>
        <h1>Key Announcements</h1>
        <p>
          Keep up with important notices and advisories that may impact your
          business.
        </p>
      </div>
      <div>
        <h1>Fines, Penalties & Seizures</h1>
        <p>
          Explore enforcement actions, including fines, to understand risks and
          stay ahead of compliance challenges
        </p>
      </div>
    </div>
    <div class="section-p">
      <div>
        <h1>Scam Alerts</h1>
        <p>
          Protect your company by staying aware of frauds and scams making waves
          in the industry.
        </p>
      </div>
      <div>
        <h1>Compliance Experts Insights</h1>
        <p>
          Gain valuable perspectives from industry compliance experts from
          leading firms
        </p>
      </div>
      <div>
        <h1>Domestic Insurance News</h1>
        <p>
          Track shifts in domestic insurance regulations to keep your business
          compliant
        </p>
      </div>
    </div>
    <div class="submit">
      <button type="button" @click="submit">Get Free Report</button>
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

  @media (max-width: 767px) {
    font-weight: 600;
    font-size: 24px;
  }
}

.section-h p {
  color: var(--color-text-secondary);
  font-weight: 400;
  font-size: 20px;

  @media (max-width: 767px) {
    font-size: 18px;
  }
}

.section-p {
  display: flex;
  flex-direction: row;
  gap: 64px;

  @media (max-width: 767px) {
    flex-direction: column;
    gap: 24px;
  }
}

.section-p div {
  display: flex;
  flex-direction: column;
  width: 100%;
  min-width: 150px;
  gap: 8px;
}

.section-p h1 {
  color: var(--color-text-primary);
  font-weight: 600;
  font-size: 20px;

  @media (max-width: 767px) {
    font-weight: 600;
    font-size: 18px;
  }
}

.section-p p {
  color: var(--color-text-secondary);
  font-weight: 400;
  font-size: 18px;

  @media (max-width: 767px) {
    font-size: 16px;
  }
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
</style>
