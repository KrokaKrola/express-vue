<template>
  <header class="header">
    <div class="container">
      <div class="wrapper">
        <a href="/" class="logo">
          <Logo />
          <span>Plan</span>
        </a>
        <nav>
          <a href="/dashboard"><Dashboard /><span>Dashboard</span></a>
          <a href="/calendar"><Calendar /><span>Calendar</span></a>
          <a href="/analytics"><Analytics /><span>Analytics</span></a>
        </nav>
        <div class="auth">
          <a href="#">Log in</a>
          <a href="#">Sign up</a>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import Logo from '../assets/logo.svg?inline';
import Dashboard from '../assets/dashboard.svg?inline';
import Calendar from '../assets/calendar.svg?inline';
import Analytics from '../assets/analytics.svg?inline';

export default {
  components: {
    Logo,
    Dashboard,
    Calendar,
    Analytics,
  },
};
</script>

<style lang="scss" scoped>
  .header {
    background-color: #fff;
  }
  .wrapper {
    padding: 10px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .logo {
    display: flex;
    align-items: center;
    font-size: 18px;
    color: #000;
    text-decoration: none;
    font-weight: 700;
    width: 113px;
    &:hover {
      color: #7933df;
    }
    svg {
      width: 40px;
      height: 40px;
      margin-right: 10px;
    }
  }
  nav {
    display: flex;
    align-items: center;
  }
  nav a {
    display: flex;
    align-items: center;
    margin-right: 35px;
    color: black;
    font-weight: 500;
    text-decoration: none;
    &:hover {
      color: #7933df;
    }
    &:last-of-type {
      margin-right: 0;
    }
    svg {
      width: 25px;
      height: 25px;
      margin-right: 12px;
    }
  }
  .auth {
    width: 113px;
    a {
      color: black;
      font-weight: 500;
      margin-right: 15px;
      text-decoration: none;
      &:hover {
        color: #7933df;
      }
      &:last-of-type {
        margin-right: 0;
      }
    }
  }
</style>
