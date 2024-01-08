# Vue


vt imports will build the setup for a vue page with the imports you need
computing the appState array tells vue it will be a reactive object and will redraw when items inside the array are changed

v-for="candy in candies" this is your for each to grab the whole array of items and draw them

<div v-for="house in houses"> <= grabs all the houses and draws their price
<div class="card">house.price</div>
</div>