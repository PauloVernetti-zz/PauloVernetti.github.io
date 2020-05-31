<template>
    <div class="flex-row fill-width" :style="styles">

    </div>
</template>

<script>
    export default {
        name: "HeaderBar.vue",
        props: {
            absolute: {
                type: Boolean,
                default: false
            },
            prominent: {
                type: Boolean,
                default: false
            },
            height: {
                type: [ String ],
                default: "64px"
            },
            color: {
                type: String,
                default: "#ecf0f1"
            }
        },
        computed: {
            styles() {
                let prominent = this.prominent;
                let height = this.height;
                let absolute = this.absolute;

                if (prominent) {
                    height = "136px";
                }

                return `height: ${this.height}; background-color: ${this.color}; ${ absolute ? "position: absolute" : "position: relative" };`
            }
        }
    }
</script>

<style scoped>
.headerbar {
    height: 64px
}
</style>