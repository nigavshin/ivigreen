<template>
  <header class="header">
    <div class="header__container container">
      <img
        class="header__logo"
        src="../assets/logo-ivigreen.svg"
        width="80"
        height="80"
        alt="logo-ivigreen"
      />
      <ul class="header__menu">
        <li class="header__menu-item">
          <a class="header__menu-link" href="">Products</a>
        </li>
        <li class="header__menu-item">
          <a class="header__menu-link" href="">About Ivi Green</a>
        </li>
        <li class="header__menu-item">
          <a class="header__menu-link" href="">FAQ</a>
        </li>
        <li class="header__menu-item">
          <a class="header__menu-link" href="">For educators</a>
        </li>
        <li class="header__menu-item">
          <a class="header__menu-link" href="">Blog</a>
        </li>
      </ul>
      <div class="header__box">
        <svg width="28" height="28" viewBox="0 0 28 28" fill="none">
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M16.8282 12.9776H20.5187C21.0783 12.9776 21.5179 12.5149 21.5179 11.9571C21.5179 11.3856 21.0783 10.9366 20.5187 10.9366H16.8282C16.2687 10.9366 15.829 11.3856 15.829 11.9571C15.829 12.5149 16.2687 12.9776 16.8282 12.9776ZM24.9019 5.90341C25.7146 5.90341 26.2476 6.18915 26.7805 6.81506C27.3134 7.44097 27.4067 8.33902 27.2867 9.15407L26.0211 18.0801C25.7813 19.7959 24.3424 21.06 22.6504 21.06H8.11502C6.34307 21.06 4.87754 19.6735 4.73099 17.8774L3.50528 3.04462L1.49352 2.69084C0.960598 2.5956 0.587555 2.06493 0.680816 1.52066C0.774076 0.964142 1.29367 0.595398 1.83991 0.678399L5.01744 1.16688C5.47042 1.24988 5.80349 1.62951 5.84346 2.09214L6.09659 5.14006C6.13656 5.57684 6.48296 5.90341 6.90929 5.90341H24.9019ZM7.90159 23.2106C6.78246 23.2106 5.8765 24.1358 5.8765 25.2788C5.8765 26.4082 6.78246 27.3334 7.90159 27.3334C9.00739 27.3334 9.91335 26.4082 9.91335 25.2788C9.91335 24.1358 9.00739 23.2106 7.90159 23.2106ZM22.8899 23.2106C21.7708 23.2106 20.8648 24.1358 20.8648 25.2788C20.8648 26.4082 21.7708 27.3334 22.8899 27.3334C23.9957 27.3334 24.9017 26.4082 24.9017 25.2788C24.9017 24.1358 23.9957 23.2106 22.8899 23.2106Z"
            fill="#3E468F"
          />
        </svg>
        <p class="header__box-count">0</p>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header {
  background-color: var(--background-grey);
}

.header__container {
  padding: 16px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 88px;
}

.header__menu {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header__menu-link {
  font-size: 20px;
  font-weight: 500;
  line-height: 150%;
  color: var(--text-dark);
}

.header__box {
  position: relative;
}

.header__box-count {
  position: absolute;
  top: -10px;
  right: -10px;
  width: 26px;
  height: 26px;
  border-radius: 50%;
  color: var(--text-light);
  background-color: var(--success);
  text-align: center;
}
</style>
