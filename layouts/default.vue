<template>
    <div>
        <TopNav />
        <h1>Górna część domyslna</h1>
        <slot />
        <footer>
            <div class="footer">
                <ol class="list">
                    <li>O NAS</li>
                    <li>BLOG</li>
                    <li>OPINIE</li>
                    <li>KONTAKT</li>
                </ol>
                <div class="address">
                    <span>KONTAKT</span>
                    <br />
                    <p>
                    <div class="parent">
                        <div class="div1">Adres: </div>
                        <div class="div2">ul. Obiwana Kenobiego 420 81-526 Gdynia </div>
                        <div class="div3">Nr Telefonu: </div>
                        <div class="div4">111-222-333 </div>
                        <div class="div5">E-mail: </div>
                        <div class="div6">mail@gmail.com </div>
                    </div>

                    <br />

                    <br />

                    </p>
                </div>
                <div class="logo">

                    <img src="./logoBlack.png" alt="" />
                    <br />
                    <img src="./socialBlack.png" alt="">

                </div>
            </div>
        </footer>
    </div>
</template>
<style scoped lang="scss">
.footer {
    height: 500px;
    background-color: black;
    color: white;
    font-size: 24px;
    font-weight: bold;
    display: flex;

}

.list {
    li {

        margin: 70px;

    }

    width: 25%;

    list-style: inside;

}

.address {
    margin-top: 100px;

    span {

        font-size: 36px;

    }




}

.parent {
    margin-top: 30px;
    display: grid;
    grid-template-columns: 300px 800px;
    grid-template-rows: repeat(3, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 30px;
    text-indent: 50px;
}

.div1 {
    grid-area: 1 / 1 / 2 / 2;
}

.div2 {
    grid-area: 1 / 2 / 2 / 3;
}

.div3 {
    grid-area: 2 / 1 / 3 / 2;
}

.div4 {
    grid-area: 2 / 2 / 3 / 3;
}

.div5 {
    grid-area: 3 / 1 / 4 / 2;
}

.div6 {
    grid-area: 3 / 2 / 4 / 3;
}

.logo {
    width: 20%;
}
</style>