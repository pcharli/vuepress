<template>
    <div>
        <h2>Nos bières</h2>
        <ul>
            <li v-for="beer in beers">{{beer.name}}</li>
        </ul>
    </div>
</template>

<script>
import Axios from 'axios'

export default {
    created() {
        let url = "https://api.punkapi.com/v2/beers"
    Axios
      .get(url)
      .then(response => (this.beers = response.data))
    },
    data() {
        return {
            beers: []
        }
    }
}
</script>