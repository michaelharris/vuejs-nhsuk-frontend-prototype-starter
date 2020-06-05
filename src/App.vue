<template>
  <div id="app">
    <header class="nhsuk-header" role="banner">
      <div class="nhsuk-width-container-fluid nhsuk-header__container">
        <div class="nhsuk-header__logo">
          <a class="nhsuk-header__link" href="/" aria-label="NHS homepage">
            <svg class="nhsuk-logo nhsuk-logo--white" xmlns="http://www.w3.org/2000/svg" role="presentation" focusable="false" viewBox="0 0 40 16">
              <path fill="#fff" d="M0 0h40v16H0z"></path>
              <path fill="#005eb8" d="M3.9 1.5h4.4l2.6 9h.1l1.8-9h3.3l-2.8 13H9l-2.7-9h-.1l-1.8 9H1.1M17.3 1.5h3.6l-1 4.9h4L25 1.5h3.5l-2.7 13h-3.5l1.1-5.6h-4.1l-1.2 5.6h-3.4M37.7 4.4c-.7-.3-1.6-.6-2.9-.6-1.4 0-2.5.2-2.5 1.3 0 1.8 5.1 1.2 5.1 5.1 0 3.6-3.3 4.5-6.4 4.5-1.3 0-2.9-.3-4-.7l.8-2.7c.7.4 2.1.7 3.2.7s2.8-.2 2.8-1.5c0-2.1-5.1-1.3-5.1-5 0-3.4 2.9-4.4 5.8-4.4 1.6 0 3.1.2 4 .6"></path>
              <image src="https://assets.nhs.uk/images/nhs-logo.png" xlink:href=""></image>
            </svg>

          </a>
        </div>

        <div class="nhsuk-header__content" id="content-header">

          <div class="nhsuk-header__menu">
            <button class="nhsuk-header__menu-toggle" id="toggle-menu" aria-controls="header-navigation" aria-label="Open menu" aria-expanded="false">Menu</button>
          </div>

          <div class="nhsuk-header__search">
            <button class="nhsuk-header__search-toggle" id="toggle-search" aria-controls="search" aria-label="Open search">
              <svg class="nhsuk-icon nhsuk-icon__search" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
                <path d="M19.71 18.29l-4.11-4.1a7 7 0 1 0-1.41 1.41l4.1 4.11a1 1 0 0 0 1.42 0 1 1 0 0 0 0-1.42zM5 10a5 5 0 1 1 5 5 5 5 0 0 1-5-5z"></path>
              </svg>
              <span class="nhsuk-u-visually-hidden">Search</span>
            </button>
            <div class="nhsuk-header__search-wrap" id="wrap-search">
              <form class="nhsuk-header__search-form" id="search" action="/search/" method="get" role="search">
                <label class="nhsuk-u-visually-hidden" for="search-field">Search the NHS website</label>
                <div class="autocomplete-container" id="autocomplete-container">
                  <div class="autocomplete__wrapper">
                    <div style="border: 0px; clip: rect(0px, 0px, 0px, 0px); height: 1px; margin-bottom: -1px; margin-right: -1px; overflow: hidden; padding: 0px; position: absolute; white-space: nowrap; width: 1px;">
                      <div id="search-field__status--A" role="status" aria-atomic="true" aria-live="polite"></div>
                      <div id="search-field__status--B" role="status" aria-atomic="true" aria-live="polite"></div>
                    </div>
                    <input aria-expanded="false" aria-owns="search-field__listbox" aria-autocomplete="list" aria-describedby="search-field__assistiveHint"
                      autocomplete="off" class="autocomplete__input autocomplete__input--default" id="search-field" name="q"
                      placeholder="Search" type="text" role="combobox">
                    <ul class="autocomplete__menu autocomplete__menu--inline autocomplete__menu--hidden" id="search-field__listbox"
                      role="listbox"></ul>
                    <span id="search-field__assistiveHint" style="display: none;">When autocomplete results are available use up and down arrows to review and enter to select. Touch device
                      users, explore by touch or with swipe gestures.</span>
                  </div>
                </div>

                <button class="nhsuk-search__submit" type="submit">
                  <svg class="nhsuk-icon nhsuk-icon__search" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
                    <path d="M19.71 18.29l-4.11-4.1a7 7 0 1 0-1.41 1.41l4.1 4.11a1 1 0 0 0 1.42 0 1 1 0 0 0 0-1.42zM5 10a5 5 0 1 1 5 5 5 5 0 0 1-5-5z"></path>
                  </svg>
                  <span class="nhsuk-u-visually-hidden">Search</span>
                </button>
                <button class="nhsuk-search__close" id="close-search">
                  <svg class="nhsuk-icon nhsuk-icon__close" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
                    <path d="M13.41 12l5.3-5.29a1 1 0 1 0-1.42-1.42L12 10.59l-5.29-5.3a1 1 0 0 0-1.42 1.42l5.3 5.29-5.3 5.29a1 1 0 0 0 0 1.42 1 1 0 0 0 1.42 0l5.29-5.3 5.29 5.3a1 1 0 0 0 1.42 0 1 1 0 0 0 0-1.42z"></path>
                  </svg>
                  <span class="nhsuk-u-visually-hidden">Close search</span>
                </button>
              </form>
            </div>
          </div>


        </div>


      </div>


      <nav class="nhsuk-header__navigationremove" id="header-navigation" role="navigation" aria-label="Primary navigation" aria-labelledby="label-navigation">
        <p class="nhsuk-header__navigation-title">
          <span id="label-navigation">Menu</span>
          <button class="nhsuk-header__navigation-close" id="close-menu">
            <svg class="nhsuk-icon nhsuk-icon__close" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
              <path d="M13.41 12l5.3-5.29a1 1 0 1 0-1.42-1.42L12 10.59l-5.29-5.3a1 1 0 0 0-1.42 1.42l5.3 5.29-5.3 5.29a1 1 0 0 0 0 1.42 1 1 0 0 0 1.42 0l5.29-5.3 5.29 5.3a1 1 0 0 0 1.42 0 1 1 0 0 0 0-1.42z"></path>
            </svg>
            <span class="nhsuk-u-visually-hidden">Close menu</span>
          </button>
        </p>
        <ul class="nhsuk-header__navigation-list header-fluid-list ">
          <li class="nhsuk-header__navigation-item">
            <router-link class="nhsuk-header__navigation-link" to="/">Home</router-link>
          </li>
          <li class="nhsuk-header__navigation-item">
            <router-link class="nhsuk-header__navigation-link" to="/form">Form</router-link>
          </li>
          <li class="nhsuk-header__navigation-item">
            <router-link class="nhsuk-header__navigation-link" to="/about">About</router-link>
          </li>
          <li class="nhsuk-header__navigation-item">
            <router-link class="nhsuk-header__navigation-link" to="/">Another Link</router-link>
          </li>
          <li class="nhsuk-header__navigation-item">
            <router-link class="nhsuk-header__navigation-link" to="/"> Yet Another Link</router-link>
          </li>
        </ul>
      </nav>


    </header>
    <nav class="nhsuk-breadcrumb" aria-label="Breadcrumb">
      <div class="nhsuk-width-container-fluid">
        <ol class="nhsuk-breadcrumb__list">

          <li class="nhsuk-breadcrumb__item">
            <a href="/" class="nhsuk-breadcrumb__link">Home</a>
          </li>

          <li class="nhsuk-breadcrumb__item">
            <a href="/" class="nhsuk-breadcrumb__link">Breadcrumb</a>
          </li>
        </ol>
      </div>
    </nav>

    <div class="nhsuk-width-container-fluid ">
      <main class="nhsuk-main-wrapper " id="maincontent" role="main">
        <router-view/>
      </main>
    </div>

    <footer role="contentinfo">
      <div class="nhsuk-footer" id="nhsuk-footer">
        <div class="nhsuk-width-container-fluid">
          <div class="nhsuk-grid-row">
            <div class="nhsuk-grid-column-full">
              <p class="nhsuk-u-secondary-text-color nhsuk-u-font-size-16">This website only stores the cookies that are needed to make it work. Read more about how
                <a href="/docs/cookies" class="nhsuk-footer__list-item-link">we use cookies.</a>
              </p>
            </div>
          </div>

          <div class="nhsuk-grid-row">
            <div class="nhsuk-grid-column-full">
              <h2 class="nhsuk-u-visually-hidden">Support links</h2>
              <ul class="nhsuk-footer__list">
                <li class="nhsuk-footer__list-item">
                  <a class="nhsuk-footer__list-item-link" href="/docs">Home</a>
                </li>
                <li class="nhsuk-footer__list-item">
                  <a class="nhsuk-footer__list-item-link" href="/docs/about">About and support</a>
                </li>
                <li class="nhsuk-footer__list-item">
                  <a class="nhsuk-footer__list-item-link" href="https://github.com/nhsuk/nhsuk-prototype-kit">NHS.UK prototype kit - GitHub</a>
                </li>
              </ul>

              <p class="nhsuk-footer__copyright">&copy; Crown copyright</p>
            </div>
          </div>
        </div>
      </div>
    </footer>



  </div>
</template>

<style lang="scss">
  @import "node_modules/nhsuk-frontend/packages/nhsuk";

.header-fluid-list {
  justify-content: normal
}

</style>

<script src="../node_modules/nhsuk-frontend/dist/nhsuk.min.js" defer></script>