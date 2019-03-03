<template>
    <nuxt-link :to="'/posts/' + id" class="postbox">
        <article>
            <div class="postbox-thumbnail">
                <div>
                    <div class="postbox-imglayout">
                    <div class="postbox-image" 
                    :style="{backgroundImage: 'url(' + icon + ')'}"></div>
                    </div>
                    <div class="postbox-textlayout">
                    <h4> {{title }} </h4>
                    <p> {{previewText}} </p>
                    <p style="opacity: 0.25;"> {{ footerText }} </p>
                    </div>
                    <div class="postbox-pricelayout">
                    <h4> {{ price }} </h4>
                    </div>
                </div>
            </div>
        </article>
    </nuxt-link>
</template>

<script>
export default {
    name: 'postBox',
    props: {
        id: {
            type: String,
            required: true
        },
        title: {
            type: String,
            required: true
        },
        previewText: {
            type: String,
            required: true
        },
        footerText: {
            type: String,
            reuired: true
        },
        icon: {
            type: String,
            required: true
        },
        price: {
            type: String,
            required: true
        }

    }
}
</script>

<style scrope>
article:hover {
    box-shadow: 0px 5px 14px rgba(0, 0, 0, 0.2);
}

.postbox-thumbnail h4 {
    margin-top: 0px;
    line-height: 2.5rem;
}
.postbox-pricelayout {
    width: 10%;
    float:left;
    margin-top: 10%;
}
.postbox-textlayout {
    width: 80%;
    float:left;
    padding: 0px 3%;
}
.postbox-imglayout {
    width: 10%;
    float:left;
}
article {
    box-shadow: 0px 5px 14px rgba(0, 0, 0, 0.1);
    background:#fff;
    width:30%;
    float:left;
    margin: 0 1.5% 5rem 1.5%;
    padding: 3%;
}
.postbox-image {
    height: 20px;
    position: relative;
    padding: 30%;
    box-sizing: border-box;
    background-position: center;
    background-size: contain;
    background-repeat: no-repeat;
}

@media screen and (max-width:800px) {
    article {
        width: 100%;
    }
}

@media screen and (min-width:800px) and (max-width:1050px) {
    article {
        width: 100%;
    }
    .postbox-imglayout {
    width: 34%;
    float: none;
    margin: 0 auto;
    margin-bottom: 3rem;
}
.postbox-textlayout {
    width: 100%;
}
.postbox-image {
    padding: 13%;
}
.postbox-pricelayout {
    margin-top:0;
    width:100%;
}
.postbox-thumbnail h4, .postbox-thumbnail p {
    text-align:center;
}
}

</style>
