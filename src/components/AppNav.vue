<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <nav>
        <div class="container">
            <ul>
                <li>
                    <a href="#">
                        <figure>
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                        </figure>
                        <span>DIGITAL COMICS</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <figure>
                            <img src="../assets/img/buy-comics-merchandise.png" alt="DC Merchandise">
                        </figure>
                        <span>DC MERCHANDISE</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <figure>
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="Subscripton">
                        </figure>
                        <span>SUBSCRIPTION</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <figure>
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="Comic Shop Locator">
                        </figure>
                        <span>COMIC SHOP LOCATOR</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <figure>
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="DC Power Visa">
                        </figure>
                        <span>DC POWER VISA</span>
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
nav {
    background-color: #0a7cec;
    padding: 2rem;

    ul {
        display: flex;
        align-items: center;
        justify-content: space-between;

        li {

            a {
                figure {
                    width: 50px;
                }

                display: flex;
                align-items: center;
                gap: 10px;

                span {
                    color: white;
                    font-size: 0.8rem;
                }
            }

            img {
                width: 100%;
            }
        }
    }
}
</style>