<script>
export default {
    data() {
        return {
            informations: [
                {
                    text: 'Business Seminar',
                    dateWeek: 'FRI',
                    date: 27,
                    dateRange: 'July 1, 2019 @ 8:00 am - July 1, 2021 @ 5:00 pm',
                    place: 'United States'

                },
                {
                    text: 'Politics Seminar',
                    dateWeek: 'FRI',
                    date: 27,
                    dateRange: 'November 6, 2019 @ 8:00 am - November 6, 2021 @ 5:00 pm',
                    place: 'ited Kingdom'

                },

            ]
        }
    },
}
</script>

<template>
   <div id="upcoming-events">
            <h4>UPCOMING EVENTS</h4>
            <div v-for="element in informations" class="upcoming-event">
                <div>
                    <div class="poster-date">
                        <div>{{ element.dateWeek }}</div>
                        <span>{{ element.date }}</span>
                    </div>
                </div>
                <div>
                    <h4>{{ element.text }}</h4>
                    <span class="text">
                        {{ element.dateRange }}
                        <br>
                        {{ element.place }}
                    </span>
                </div>
            </div>


            <a href="#">View More...</a>
        </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

#upcoming-events {


    h4 {
        padding-bottom: 20px;
    }

    .upcoming-event {
        display: flex;
        padding: 20px 0;
        border-bottom: $textGray solid 1px;

        .poster-date {
            background-color: $primaryColor;
            width: 70px;
            height: 90px;
            text-align: center;
            padding: 5px;
            margin-right: 20px;

            div {
                background-color: #eff0f2;
                width: 60px;
                height: 50px;
                color: $primaryColor;
                font-weight: 400;
                display: flex;
                justify-content: center;
                align-items: center;
                margin-bottom: 7px;
            }

            span {
                color: $thirdColor;
                font-size: 18px;
                font-weight: 500;

            }
        }

        .text {
            color: $textGray;
        }

    }

    a {
        color: black;
        padding-top: 20px;
        display: flex;
        color: $textGray;
        font-weight: 300;
    }

}
</style>