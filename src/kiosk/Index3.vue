<template>
    <div>
        <div class="q-pa-md q-gutter-sm">
            <transition
                    appear
                    enter-active-class="animated fadeIn"
                    leave-active-class="animated fadeOut"
            >




            </transition>
            <q-img v-show="this.index"
                   class="shadow-up-3"
                   :src="require('./monte.jpg')"
                   spinner-color="white"
                   style="height: 540px; max-width: 1000px;margin-left: 9%"
            />
            <Plot/>
            <q-img
                    v-show="this.area.A"
                    class="shadow-up-3"
                    :src="require('./a.jpg')"
                    spinner-color="white"
                    style="height: 540px; max-width: 1000px;margin-left: 9%"
            />


            <q-img
                    v-show="this.area.B"
                    class="shadow-up-3"
                    :src="require('./b.jpg')"
                    spinner-color="white"
                    style="height: 540px; max-width: 1000px;margin-left: 9%"
            />

            <q-img
                    v-show="this.area.C"
                    class="shadow-up-3"
                    :src="require('./c.jpg')"
                    spinner-color="white"
                    style="height: 540px; max-width: 1000px;margin-left: 9%"
            />

            <q-img
                    v-show="this.area.D"
                    class="shadow-up-3"
                    :src="require('./d.jpg')"
                    spinner-color="white"
                    style="height: 540px; max-width: 1000px;margin-left: 9%"
            />

            <q-img
                    v-show="this.area.E"
                    class="shadow-up-3"
                    :src="require('./e.jpg')"
                    spinner-color="white"
                    style="height: 540px; max-width: 1000px;margin-left: 9%"
            />

            <q-img
                    v-show="this.area.F"
                    class="shadow-up-3"
                    :src="require('./f.jpg')"
                    spinner-color="white"
                    style="height: 540px; max-width: 1000px;margin-left: 9%"
            />


            <q-img
                    v-show="this.area.g"
                    class="shadow-up-3"
                    :src="require('./g.jpg')"
                    spinner-color="white"
                    style="height: 540px; max-width: 1000px;margin-left: 9%"
            />

            <q-img
                    v-show="this.area.H"
                    class="shadow-up-3"
                    :src="require('./h.jpg')"
                    spinner-color="white"
                    style="height: 540px; max-width: 1000px;margin-left: 9%"
            />
        </div>
            <Notif/>

    </div>
</template>

<script>
    import {mapState} from 'vuex'
    import Notif from "./Notif";
    import Plot from "./Plot";
    export default {
        components: {Plot, Notif},
        methods: {

        },

        computed:mapState({
            area:state => state.index3.areaImg,
            index:state => state.index3.showImg
        })


    }
</script>

<style scoped>

</style>