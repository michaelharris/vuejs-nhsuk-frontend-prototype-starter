<template>
  <div class="form">

    <div class="nhsuk-grid-row">
      <div class="nhsuk-grid-column-two-thirds">
        <h1>
          Find a dentist
        </h1>


        <div class="nhsuk-inset-text">
          <span class="nhsuk-u-visually-hidden">Information: </span>
          <p>Because of coronavirus (COVID-19), all routine dental treatment has been stopped at the moment.</p>
          <p>If you think you need urgent dental treatment:</p>
          <ul class="nhsuk-list nhsuk-list--bullet">
            <li>call your dentist</li>
            <li>use the
              <a href="https://111.nhs.uk/">NHS 111 online service</a> if you cannot contact your dentist or you do not have one</li>
          </ul>
        </div>


        <form name="ServiceSearchForm" id="service-search-form" method="post" action="/service-search/find-a-dentist">
          <input type="hidden" value="DEN" data-val="true" data-val-required="The ServiceId field is required." id="ServiceId" name="ServiceId"
          />
          <input type="hidden" id="UsersLatitude" name="UsersLatitude" value="" />
          <input type="hidden" id="UsersLongitude" name="UsersLongitude" value="" />
          <div class="nhsuk-form-group">
            <label class="nhsuk-label" for="Location">
              Enter a town, city or postcode in England
            </label>
            <input class="nhsuk-input nhsuk-input--width-20" type="text" id="Location" name="Location" value="">
          </div>
          <button class="nhsuk-button nhsuk-u-margin-bottom-4" type="submit">Search</button>
          <br />
          <button class="nhsuk-button nhsuk-button--secondary geo-locate--button nhsuk-u-margin-bottom-7">Use your location</button>
          <div class="geo-locate">
            <p class="geo-locate--searching nhsuk-u-margin-bottom-7">
              <img src="/service-search/dist/images/loading.gif" alt="" />We are searching for your location</p>
            <p class="geo-locate--error nhsuk-u-margin-bottom-7">We can't find your location. Please try again or enter a town, city or postcode.</p>
            <p class="geo-locate--denied nhsuk-u-margin-bottom-7">You have not allowed us to use your location. You can change this in your browser settings.</p>
          </div>
          <input name="__RequestVerificationToken" type="hidden" value="CfDJ8IyMLXMAgG5On8nD941wbV919UXhSYiZzgCdQM8YsKe5qeTq_hx_m1RSqf9cvt3hgaOATeC8ttT-BNiuC9_LPI0BlkSGU785cEm316wM5CKsJUeDHCIGlxacpBDwXSwn7_QXn5YpqclXBfqEjEjkMAM"
          />
        </form>


      </div>
    </div>

  </div>
</template>