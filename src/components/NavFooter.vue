<script>
export default {

}
</script>

<template>
    <div class="cotainerBackground">


    <div id="bottomFooter">
        <div >
            <h4>AVADA UNIVERSITY</h4>
            <a class="contact-university" href="#">
                <font-awesome-icon icon="fa-solid fa-house-chimney" class="font-icon"/>
                Residential Location 9521 Broadsberry Avenue Paddington RC7 9ZA
            </a>
            <a class="contact-university" href="#">
                <font-awesome-icon icon="fa-solid fa-phone-flip" class="font-icon"/>
                1.800.5678910
            </a>
            <a class="contact-university" href="#">
                <font-awesome-icon icon="fa-solid fa-envelope" class="font-icon"/>
                info@your-domain.com
            </a>
            <a class="contact-university" href="#">
                <font-awesome-icon icon="fa-regular fa-clock" class="font-icon"/>
                Monday - Friday: 8:00 AM - 10:00 PM
            </a>
        </div>


        <div id="recent-posts">
            <h4>RECENT POSTS</h4>
            <a href="#">
                <font-awesome-icon icon="fa-solid fa-chevron-right" class="font-icon"/>
                <div>    
                    What do successful grads think you should study?
                    <span class="date-post">March 16, 2016</span>
                </div>
            </a>
            <a href="#">
                <font-awesome-icon icon="fa-solid fa-chevron-right" class="font-icon"/>
                <div>
                    Former student discusses success in the fashion industry
                    <span class="date-post">March 15, 2016</span>
                </div>
            </a>
            <a href="#">
                <font-awesome-icon icon="fa-solid fa-chevron-right" class="font-icon" />
                <div>
                    
                    How do you best prepare for university?
                    <span class="date-post">March 15, 2016</span>
                </div>
            </a>
            
        </div>

        <div class="navBrowswer">
            <h4>COURSES</h4>
            <a href="#">Arts & Humanities</a>
            <a href="#">Busines & Menagement</a>
            <a href="#">Engineering & Tecnology</a>
            <a href="#">Life Sciences & Medicine</a>
            <a href="#">Natural Scienses</a>

            <h4 id="secondNavElement">ADMISSIONS</h4>
            <a href="#">Eligibility</a>
            <a href="#">Application</a>
            <a href="#">Review Process</a>
            <a href="#">How to Apply</a>
        </div>


        <div class="navBrowswer">
            <h4>RESOURCES</h4>
            <a href="#">Campus Directory</a>
            <a href="#">Academic Calendar</a>
            <a href="#">Sport Clubs</a>
            <a href="#">Graduate Programs</a>
            <a href="#">Faculty & Staff</a>

            <h4 id="secondNavElement">QUICKLINKS</h4>
            <a href="#">University Library</a>
            <a href="#">Campus</a>
            <a href="#">Careers</a>
        </div>

        <div id="upcoming-events">
            <h4>UPCOMING EVENTS</h4>
            <div class="upcoming-event">
                <div>
                    <div class="poster-date">
                        <div>FRI</div>
                        <span>27</span>
                    </div>
                </div>
                <div>
                    <h4>Business Seminar</h4>
                    <span class="text">
                        July 1, 2019 @ 8:00 am - July 1, 2021 @ 5:00 pm
                        <br>
                        United States
                    </span>
                </div>
            </div>


            <div class="upcoming-event">
                <div>
                    <div class="poster-date">
                        <div>FRI</div>
                        <span>27</span>
                    </div>
                </div>
                <div>
                    <h4>Politics Seminar</h4>
                    <span class="text">
                        November 6, 2019 @ 8:00 am - November 6, 2021 @ 5:00 pm
                        <br>
                        United Kingdom
                    </span>
                </div>
            </div>

            <a href="#">View More...</a>
        </div>
    </div>
</div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

.cotainerBackground {
    background-image: url('/images/university_ft_bg.png');
    background-position: -250px;


    #bottomFooter {
        max-width: 1300px;
        margin: 0 auto;

        display: flex;
        justify-content: space-between;

        padding: 70px 30px 30px;
        font-size: 13px;

        &>div {
            width: calc((100% / 5) - 30px);
            margin: 0 15px;

            h4 {
                padding-bottom: 20px;
            }

            .contact-university {
                padding-bottom: 20px;
            }

            a {
                display: flex;
                color: #767e85;
                font-weight: 300;

                .font-icon {
                    padding-right: 10px;
                }
            }

            &.navBrowswer {
                a {
                    line-height: 23px;
                }
            }

            #secondNavElement {
                padding-top: 30px;
            }
        }

        #recent-posts {
            a {
                align-items: baseline;
                padding-top: 10px;

                .font-icon {
                    font-size: 10px;
                    vertical-align: baseline;
                }

                div {

                    line-height: 25px;
                    border-bottom: 1px solid #767e85;
                    padding-bottom: 10px;
                    color: black;

                    .date-post {
                        display: block;
                        color: #767e85;
                    }
                }
            }
        }

        #upcoming-events {


            .upcoming-event {
                display: flex;
                padding: 20px 0;
                border-bottom: #767e855a solid 1px;

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
                    color: #767e85;
                }

            }

            a {
                color: black;
                padding-top: 20px;
            }
        }
    }
}
</style>