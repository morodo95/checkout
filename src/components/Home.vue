<template>
    <div class="main-wrapper">

        <section class="section">
            <div class=" bd-main-container  container ">
                <nav class="level is-mobile">
                    <div class="level-item has-text-centered">
                        <div>
                            <p class="heading">Tweets</p>
                            <p class="title">3,456</p>
                        </div>
                    </div>
                </nav>
                <article class="media">
                    <div class="media-content">
                        <div class="content">
                            <p>
                                <strong>John Smith</strong> <small>@johnsmith</small> <small>31m</small>
                                <br>
                                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin ornare magna eros, eu
                                pellentesque tortor vestibulum ut. Maecenas non massa sem. Etiam finibus odio quis
                                feugiat
                                facilisis.
                            </p>
                        </div>
                        <nav class="level is-mobile">
                            <div class="level-left">
                                <a class="level-item">
                                    <span class="icon is-small"><i class="fas fa-user"></i></span>
                                </a>
                                <a class="level-item">
                                    <span class="icon is-small"><i class="fas fa-retweet"></i></span>
                                </a>
                                <a class="level-item">
                                    <span class="icon is-small"><i class="fas fa-heart"></i></span>
                                </a>
                                
                            </div>
                        </nav>
                    </div>
                </article>
            </div>
        </section>
    </div>
</template>
<script>
    export default {
        data() {
            const today = new Date()
            return {
                dates: [],
                minDate: new Date(today.getFullYear(), today.getMonth(), today.getDate()),
                maxDate: new Date(today.getFullYear(), today.getMonth(), today.getDate() + 356),
                carousels: [{
                        text: 'Slide 1',
                        color: 'primary'
                    },
                    {
                        text: 'Slide 2',
                        color: 'info'
                    },
                    {
                        text: 'Slide 3',
                        color: 'success'
                    },
                    {
                        text: 'Slide 4',
                        color: 'warning'
                    },
                    {
                        text: 'Slide 5',
                        color: 'danger'
                    }
                ]
            }
        },
        mounted() {
            console.log(process.env);
        },

    }
</script>