<template>
  <header>
    <navbar>
      <div class="logo">
        <img class="logo__image" src="@/assets/images/logo.png" alt="logo">
        <span class="logo__text">
          <h5 class="logo__text-title">Daily Interview</h5>
          <h6 class="logo__text-subtitle">FAANG questions and articles</h6>
        </span>
      </div>
    </navbar>
  </header>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";

export default defineComponent({
  name: "v-header",
})
</script>

<style lang="scss" scoped>
header {
  navbar {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;

    .logo {
      display: flex;
      flex-direction: row;
      align-items: center;
      justify-content: flex-start;

      .logo__image {
        width: 55px;
        height: 55px;
      }

      .logo__text {
        margin-left: .5rem;

        .logo__text-title {
          font-size: 2.4rem;
          font-weight: bold;
          letter-spacing: 1.1px;
        }

        .logo__text-subtitle {
          font-size: 1.8rem;
          font-weight: 400;
        }
      }
    }
  }
}
</style>
