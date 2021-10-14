<template>
    <div class="header_bottom cflex">
        <div class="cflex">
            <h1>Contemporary Ideas</h1>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Reiciendis nostrum natus hic est ab recusandae, facilis repellat eveniet unde praesentium, doloribus ratione sint! Repudiandae perspiciatis sit molestiae commodi.</p>
            <div class="header_button flex">
                <button>REGISTER NOW</button>
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
    $principalColor : #40c4ff;
    $textColor : white;
    .header_bottom {
        height: calc(100vh - 80px);
        /* per non applicare l'opacity all'elemento */
        position: relative;
        color: $textColor;
        div {
            width: 80%;
            margin: auto;
            h1 {
                font-size: 80px;
            }
            p {
                text-align: center;
                font-size: 20px;
            }
            button {
                margin: auto;
                padding: 18px 60px;
                border: none;
                font-weight: 500;
                &:hover {
                    color: $textColor;
                    background-color: $principalColor;
                }
            }
        }
        h1, p, .header_button {
                margin: 20px auto;
            }
    }
</style>