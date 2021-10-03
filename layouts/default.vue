<template>
    <div>
        <div class="row">
            <div class="col-md-12 p-0">
                <FrontNavbar/>
            </div>
        </div>
        <div class="row body-web">
            <div class="col-md-12">
                <Nuxt />
            </div>
        </div>
    </div>
</template>

<script>

export default {

    data() {
        return {
        }
    },
    head() {
        return {
            htmlAttrs: {
                lang: "es",
            },
            titleTemplate: "Smart Teach ",
            link: [
                {
                    rel: "stylesheet",
                    href: "https://fonts.googleapis.com/css?family=Oswald&display=swap",
                },
            ],
            metaInfo: {
                meta: [
                    { charset: "utf-8" },
                    {
                        name: "viewport",
                        content: "width=device-width, initial-scale=1, shrink-to-fit=no",
                    },
                ],
            },
        };
    },
    methods: {
    },
    mounted() {
    }
};
</script>

<style>
.row{
    margin: 0px;
    padding: 0px;
}
.body-web{
    background-color: #192954;
    color: #ffffff;
}
.foro-item img{
    border-radius: 40px;
    overflow: hidden;
}
</style>