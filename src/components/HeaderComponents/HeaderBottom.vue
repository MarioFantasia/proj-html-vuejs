<template>
    <div class="header_bottom cflex">
        <div class="cflex">
            <h2>SCRITTA GRANDE</h2>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Reiciendis nostrum natus hic est ab recusandae, facilis repellat eveniet unde praesentium, doloribus ratione sint! Repudiandae perspiciatis sit molestiae commodi quibusdam ipsum.</p>
            <div class="header_button flex">
                <button>register now</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'HeaderBottom'
}
</script>

<style lang="scss" scoped>
    .header_bottom {
        height: calc(100vh - 80px);
        position: relative; /* per non applicare l'opacity all'elemento */
        color: white;
        div {
            width: 60%;
            margin: auto;
            h2, p, .header_buttom {
                margin: auto;
            }
            button {
                margin: auto;
            }
        }
    }
</style>