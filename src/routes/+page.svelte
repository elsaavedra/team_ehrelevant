<script>
	import k12 from '$lib/images/K12-banner1.jpg';
    import a1 from '$lib/images/question_1a_plot1.png';
    import b1 from '$lib/images/question_1b_plot1.png';
    import c1 from '$lib/images/question_1c_plot1.png';
    import a2 from '$lib/images/question_2a_plot1.png';
    import b2 from '$lib/images/question_2b_plot1.png';
    import c2 from '$lib/images/question_2c_plot1.png';
    import hyp from '$lib/images/hypothesis_testing.png';
</script>

<body>
    <ul class="navbar">
        <a id="sussy" href="#Amogus" style="font-family: Times New Roman"> team_ehrelevant </a>
        <a href="#Introduction">Introduction</a>
        <a href="#DataRepo">Data Repository</a>
        <a href="#DataVisual">Data Visualization</a>
        <a href="#Conc">Conclusion</a>
    </ul>
    
    <section class="content">
    <!-- svelte-ignore a11y-distracting-elements -->
    <marquee scrollamount=30 id="Introduction">team_ehrelevant says hello world</marquee>
    
    <section>
        <div>
            <p id="quote">Education is not preparation for life; Education is life itself.</p>
            <p style = "text-align: right; font-size: 1.5em"> - John Dewey</p> 
        </div>
        
        <p id="sub"> 
            Truly, it is quite evident that one's education strongly influences the kind of life that one lives.
            Various reasons one may have to further their education, whether it is to apply for practical knowledge or deepen their understanding in specialized fields, but one thing remains the same; education.
            However, one's education, strictly focusing on the schooling aspect of education, isn't necessarily applicable to one's field of work.
            This may be due to many reasons such as a shift in interest, a cruel demand in one's specialization, or simply the lack of available jobs.
        </p>
        
        <section class="wrapper4">
            <div class="image">
                <img src={k12} alt="K-12 Banner" style="
                width: 40vw;
                padding: 1em;
                border-radius: 25px;">
                <p style="display: inline;">Source: <a href="https://thepost.net.ph/news/nation/k-12-a-legacy-of-pnoy-deped">The Post Ph</a></p>
            </div>

            <div id="sub">
                <p class="intro2">
                    In the Philippines, one such shift in education would be the implementation of the K-12 basic education curriculum in 2012.
                    This change was an attempt to improve current schooling to bring up “job-ready” students after graduating their 12th grade.
                    Despite the improvement in their Math and Science subjects, most major companies in the Philippines would still prefer college graduates over high school graduates.<sup><a href="https://www.philstar.com/headlines/2023/05/12/2265854/deped-forms-task-force-employability-issues-senior-high-graduates">[1]</a></sup>
                    Most K-12 graduates that were lucky enough to be employed receive only minimum wage for entry-level positions while college graduates receive many more benefits than this.<sup><a href="https://www.philstar.com/headlines/2023/12/04/2316419/most-job-vacancies-accepting-senior-high-grads-offer-minimum-wage-work-dole">[2]</a></sup>
                    This heavily contrasts one of the main objectives of K-12 to “produce employable students as early as post-high school”. <sup><a href="https://www.philstar.com/headlines/2023/05/12/2265854/deped-forms-task-force-employability-issues-senior-high-graduates">[3]</a></sup>
                </p>
            </div>
        </section>
    </section>

    <section class="wrapper">
        <div class="box1">
            <h2> Problem </h2>
                <p>
                    Graduates in the Philippines, specifically senior high school graduates of the
                    K-12 basic education, are being discriminated against in terms of employment.
                </p>
        </div>

        <div class="box2">
            <h2> Solution </h2>
                <p>
                    The goal of this research is to use data science to analyze the actual importance
                    of knowledge gained in school across different fields and possible benchmarks
                    for useful knowledge, in turn finding practical solutions to employ K-12 graduates.
                </p>
        </div>

        <div class="box3">
            <h2> Objectives </h2>
                <p id="sub2">Does the level of participation of Filipinos in different fields of expertise correlate with their highest level of educational attainment?</p>
                <p id="sub2">Across different fields of expertise, how useful is knowledge learned from school to Filipinos seeking jobs?</p>
        </div>
    </section>

    
    <section class="wrapper2">
        <div class="box11">
            <p style="text-align: center; padding: 10px; font-size: 30px"> Hypothesis #1</p>       
            <h3> Null Hypothesis </h3>
                    <p id="sub2">
                        The level of participation of Filipinos in different fields of expertise does not correlate to their highest level of educational attainment.
                    </p>

                <h3> Alternative Hypothesis </h3>
                    <p id="sub2">
                        The level of participation of Filipinos in different fields of expertise correlates to their highest level of educational attainment.
                    </p>
        </div>
        <div class="box12">
            <p style="text-align: center; padding: 10px; font-size: 30px"> Hypothesis #2</p>    
            <h3> Null Hypothesis </h3>
                    <p id="sub2">
                        Across each field of expertise, the perceived usefulness of knowledge learned from school by Filipinos has no correlation with their level of participation in that field.
                    </p>

                <h3> Alternative Hypothesis </h3>
                    <p id="sub2">
                        The perceived usefulness of knowledge learned from school by Filipinos has a correlation with their level of participation in some or all of the specified fields of expertise.
                    </p>
        </div>

    </section>

    <section id="DataRepo">
    <h1 style="font-size: 30px;"> Dataset Description </h1>
        <section id="sub1">
            <h2 style="color: #03042d;"> Dataset Source: FLEMMS 2019 </h2>
                <p id="sub3">
                    The Philippine Statistics Authority (PSA) organizes a survey known as the <a href = "https://psada.psa.gov.ph/catalog/FLEMMS/about"> Functional Literacy, Education and Mass Media Survey (FLEMMS) </a> as a regular check on the state of the country's education systems.
                    FLEMMS collects general information about each respondent's educational background, demographic information, and household information, followed by questions to ask and assess their ability to read, write, and answer questions.
                    These assessments are then interpreted to classify each respondent's educational skills through a metric known as the Functional Literacy [Level].

                    As of April 2024, the most updated results available for the FLEMMS survey are those from the FLEMMS 2019 survey, whose report may be found through <a href="https://lcc.deped.gov.ph/ls-flemms/"> this link </a>.
                </p>
        </section>

        <section id="sub1">
            <h2 style="color: #03042d;"> Data Collection </h2>
                <p id="sub3"> 
                    The results of the FLEMMS 2019 survey are divided into several CSV (Comma Separated Value) files tabulating the information gathered from each respondent.
                    Among the files, this study intends to investigate the data from the responses in the Household Name CSV file. The Household Name CSV contains the respondents' answers to the Individual Questionnaire, which contains questions that directly assess their educational background and overall literacy.
                    The relevant files for the FLEMMS 2019 dataset can be downloaded from the <a href="https://psada.psa.gov.ph/catalog/FLEMMS/about"> Philippine Statistics Authority Data Archive (PSADA) website </a>.
                </p>
        </section>

        <section id="sub1">
            <h2 style="color: #03042d;"> Data Preprocessing </h2>
                <div id="sub3">
                    <p> 
                        From the Household Name CSV, the first few fields are kept to uniquely identify each of the data points of the dataset, namely the Region (REG), Urbanity (URB), Household ID (HHID), and the Respondent Line Number (RESP_LNO).
                    </p>
                    <br>
                    <p> 
                        Furthermore, certain fields were found to be the most relevant to the study as variables to be kept, namely the 
                        <li> Level of Participation (Q15A_ARTS, Q15B_SCIENCE, Q15C_BUSINESS), </li>
                        <li> Knowledge in Job (Q21_KNOWLEDGE), and </li>
                        <li> Highest Educational Attainment (C12_HEA_RT04). </li>
                        <br><br>
                        Other than these, other “potentially useful” fields were also kept for possible sub-correlation or confounding variables, which include 
                        <li> the Technical-Vocational Variables (Q5_TECHVOC, Q5_TECHVOC_COURSE, Q5_SPECIFY_COURSE), </li>
                        <li> the TESDA National Certification (Q6_TESDA_CERT), </li>
                        <li> Activities to help other people (Q20_ACTIVITY), Age (C5_AGE_RT04), Sex (C4_SEX_RT04), and </li>
                        <li> Ongoing School Status (C14_ATTEND_SCHOOL_RT04). </li>
                    </p>
                    <br>
                    <p> 
                        As such, the above-mentioned variables are kept in the “specific variables” to be used for the study, with any other columns deleted from the dataset. Nonetheless, both this reduced dataset and the full dataset may be found in the link below, for viewing reference.
                    </p>
                </div>
        </section>

        <section id="sub1">
        <h2 style="color: #03042d;"> Dataset Link </h2>
            <div id="sub3">
                <p><a href="https://docs.google.com/spreadsheets/d/1wG50_tLEtZrU1jB0AkM7doo6a6njIig8xorNHGk05Ig/edit#gid=1228805475">Here</a> is a link to the datasheet that will be used for this research. This contains the following: </p>
                <br>
                <ul>
                    <li>Selected questions from FLEMMS 2019 dataset to be analyzed</li>
                    <li>Dictionary of selected questions from FLEMMS 2019 dataset to be analyzed</li>
                    <li>Full unedited FLEMMS 2019 dataset</li>
                    <li>Dictionary of the unedited FLEMMS 2019 dataset</li>
                </ul>
            </div>
        </section>
    </section>

    <section id="DataVisual">
        <h1> Visualization of Data </h1>
        <section id="sub3">
            <p style="text-align:justify">
                Here we have three box plots which plots the participant's highest educational attainment against their level of participation. 
                The left-most, middle, and right-most plots correspond to the participants' participation in the Arts, Sciences, and Business respectively.
                <br><br>
                The specifics of each level of participation and educational attainment is discussed below.
                <br><br>
                The "boxes" in the plot corresponds to the frequency of answers for each category. 
                This means that each column's width is only respective to itself and not globally related. 
                It's important to note that most respondents are under the junior high school and bachelor categories, with the other categories having significantly less respondents compared to these two. 
                <br><br>
                For the arts, we can see a general upward trend between higher educational attainment and level of participation. 
                This suggests that education is seen to be closely related to the level of one's participation in the field of arts. 
                This suggest that to feel more involved in art, a higher educational attainment would be better.
                <br><br>
                For sciences, there's also a general upward trend, similar to the arts, where a higher level of educational attainment allows one to feel more involved. 
                It is interesting to note that those who only received an early childhood education has responses evenly spread out from 1–4. 
                This either suggest that the participant is not aware of the full scale of their participation, or that more education does not necessarily equate to more participation
                <br><br>
                Finally, for business, it's interesting to see that after finishing highschool and your bachelor's degree, there is a general downward trend in level of participation. 
                This may suggest that further education after your bachelor's degree will actually decrease your level of participation.
            </p>
        </section>

        <section class="wrapper3">
            <section id="sub4">
                <img src={a1} alt="Participation in Arts" class="center" style='border-radius: 25px; margin: 5px'>
                <p style="text-align:center">Level of Participation in Arts vs Highest Educational Attainment</p>
            </section>
            <section id="sub4">
                <img src={b1} alt="Participation in Science" class="center" style='border-radius: 25px; margin: 5px'>
                <p style="text-align:center">Level of Participation in Science vs Highest Educational Attainment</p>
            </section>
            <section id="sub4">
                <img src={c1} alt="Participation in Business" class="center" style='border-radius: 25px; margin: 5px'>
                <p style="text-align:center">Level of Participation in Business vs Highest Educational Attainment</p>
            </section>
        </section>

        <section id="sub3">
            <p>
                Here we have three violin plots which plots the participant's level of participation against their percieved usefulness of knowledge. 
                The left-most, middle, and right-most plots correspond to the participants' participation in the Arts, Sciences, and Business respectively.
                <br><br>
                The specifics of each level of participation is discussed below. Meanwhile, 1 corresponds to yes (Knowledge IS useful) and 2 corresponds to no (Knowledge is NOT useful). There are no values in between despite the visuals suggesting so. 
                <br><br>
                Similar to the box plot, each "swell" in the plot corresponds to the frequency of answers for each category. This means that each column's width is only respective to itself and not globally related.
                <br><br>
                For all three categories—the arts, sciences, and business—we can see a general larger swell in the perceived usefulness of knowledge with a score of 1 as level of participation increases. 
                At a level of participation score of 1, we can see a roughly equal score of perceived usefulness of knowledge, with this knowledge generally becoming more useful with higher levels of participation.
                <br><br>
                For the arts, specifically, we see the highest frequency with a level of participation score of 4. 
                <br><br>
                For science, we see the highest frequency with a level participation score of 4, with 3 not differing by much. 
                <br><br>
                For business, we see the highest frequency with a level participation score of 5. It is also interesting to note that those who perceive their knowledge as not useful is thicker compared to the arts and sciences for each level. This may suggest that knowledge is perceived as not as useful for business as compared to art and science.</p>
        </section>

        <section class="wrapper3">
            <section id="sub4">
                <img src={a2} alt="Knowledge in Arts" class="center" style='border-radius: 25px; margin: 5px'>
                <p style="text-align:center">Perceived Usefulness of Knowledge vs Level of Participation in Arts</p>
            </section>
            <section id="sub4">
                <img src={b2} alt="Knowledge in Science" class="center" style='border-radius: 25px; margin: 5px'>
                <p style="text-align:center">Perceived Usefulness of Knowledge vs Level of Participation in Science</p>
            </section>
            <section id="sub4">
                <img src={c2} alt="Knowledge in Business" class="center" style='border-radius: 25px; margin: 5px'>
                <p style="text-align:center">Perceived Usefulness of Knowledge vs Level of Participation in Business</p>
            </section>
        </section>
    </section>

    <section>
        <h1> Hypothesis Testing </h1>
        <div class="wrapper" id="sub1">
        <section id="box1" class="image">
            <div>
                <img src={hyp} alt="Hypothesis Testing" class="center" style='width: 100%'>
                <p style="text-align:center">Significance of First Hypothesis Across Different Fields</p>
            </div>
        </section>
        <section id="box2">
            <p> Hypothesis testing was done for the first objective, determining the correlation between the respondents' Level of Participation in different fields of expertise and their Highest Level of Educational Attainment. 
                Each of these variables is defined on an ordinal scale, with their values as follows: </p>
            
            <br>
            <p>Highest Level of Educational Attainment</p>
            <ul>
                <li> 0 (Did not study) </li>
                <li> 1 (Early Childhood Education) </li>
                <li> 2 (Elementary School) </li>
                <li> 3 (Junior High School) </li>
                <li> 4 (Senior High School) </li>
                <li> 5 (Post-Secondary Non-Tertiary) </li>
                <li> 6 (Short-cycle Tertiary) </li>
                <li> 7 (Bachelor or eqv.) </li>
                <li> 8 (Master or eqv.) </li>
                <li> 9 (Doctorate or eqv.) </li>
            </ul>
            <br>
            <p>Level of Participation A (Arts and Performance)</p>
            <ul>
                <li> 5 (Always) </li>
                <li> 4 (Often) </li>
                <li> 3 (Sometimes) </li>
                <li> 2 (Rarely) </li>
                <li> 1 (Never) </li>
            </ul>
            <br>
            <p>Level of Participation B (Science and Technology)</p>
            <ul>
                <li> 5 (Always) </li>
                <li> 4 (Often) </li>
                <li> 3 (Sometimes) </li>
                <li> 2 (Rarely) </li>
                <li> 1 (Never) </li>
            </ul>
            <br>
            <p>Level of Participation C (Work and Business) </p>
            <ul>
                <li> 5 (Always) </li>
                <li> 4 (Often) </li>
                <li> 3 (Sometimes) </li>
                <li> 2 (Rarely) </li>
                <li> 1 (Never) </li>
            </ul>
        </section>
        </div> 
    </section>

    <section id="Conc">
        <h1> Conclusion </h1>
        <section id="sub3">
            <p style="text-align:justify">
                We primarily focused on addressing the first objective and hypothesis, which was achieved through statistical testing.
                We have achieved a p-value lower than 0.005 for all three fields—the arts, sciences, and business. This means that the results are all statistically significant for all three fields.
                This also means that we reject the null hypothesis. As such, the level of participation of Filipinos is correlated to their highest level of educational attainment across all three fields of expertise.
            </p>
        </section>

        <section id="sub3">
            <p style="text-align:justify">
                Moving forward with this project, data used to conduct this study is actually quite limited and skewed across different categories of highest educational attainment. 
                More than half of the participants' highest educational attainment is junior highschool with bachelor or eqv. taking a majority of what remains. 
                Although unlikely, more data across different aspects of education would be best to better understand the distribution of responses.</p>
            <br><br>
            <p style="text-align:justify">
                Furthermore, machine learning can also be utilized in order to interpret the data as well, through data classification. 
                Each objective can be studied with a neural network that attempts to predict the dependent variable based on set feature variables. 
                For instance, the first model can attempt to determine an individual's most probable level of participation in each of Arts, Science, and Business using a classification model, which can be implemented using libraries such as TensorFlow and Keras.
                These level of participation may be predicted by the model based on the individuals':
            </p>
            <br>
                <ul>
                    <li> highest level of educational attainment </li>
                    <li> other demographic information </li>
                    <li> personal values </li>
                    <li> experiences with sports </li>
                    <li> exposure to communication media </li>
                    <li> etc. </li>
                </ul>
        </section>
    </section>

    <section id="Amogus">
        <h1 style="text-align:center">About Us</h1>
        <section class="wrapper3">
            <div class="about1">
                <h1 style="text-align:center">Edzo Acyatan</h1>
                <p style="font-size: 15; text-align: center">
                    Hey hi hello, Edzo here! I'm a 2nd year CS student of UP Diliman (as of writing this intro). I've always enjoyed playing games, and 
                    it felt like the next natural step for me was learning where these games come from. I enjoy making my code as efficient (and short) as it could be. <br> <br>

                    Besides all the computer science stuff, I'm an avid reader of Manhwa (mostly on Webtoons). I also enjoy making people disappointed with my cheesy and dry humor.
                </p>
                <p style="text-align:center"> <br> <br> <br> csacyatan1@up.edu.ph</p>
            </div>
            <div class="about2">
                <h1 style="text-align:center">Lawrence Bermudez</h1>
                <p style="font-size: 15; text-align: center">
                    Good morning there! I am Lawrence, a 2nd year Computer Science student at UP Diliman. I enjoy programming casually, whether for games or for just appreciating the logic with how programs work. <br> <br>
                    With the little time I usually have, I generally play lighter games such as rhythm games, especially osu!. <br> <br>
                    You may contact me through my email below, or through my IP at [REDACTED]. See you!
                </p>
                <p style="text-align:center"> <br> <br> <br> drbermudez1@up.edu.ph</p>
            </div>
            <div class="about3">
                <h1 style="text-align:center">Yuwen Saavedra</h1>
                <p style="font-size: 15; text-align: center"> 
                    o/ Hi! I'm Yuwen and I am a 2nd year Computer Science student at UP Diliman. I like video games (a little bit too much) so now I'm in the CS world! <br> <br>
                    Other than malding over terrible gacha rates ingame, I mostly spend the day finishing requirements and dipping my hands into projects relating to Computer Science such Front-End Web development and game development.
                    I also enjoy watching vtubers in my spare time (go watch <a href="https://www.youtube.com/@TakaneLui">Takane Lui</a>).
                </p>
                <p style="text-align:center"> <br> <br> <br> elsaavedra@up.edu.ph</p>
            </div>
        </section>
    </section>
</section>
</body>

<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
        color: #FFF;
    }

    /* Cursor Wheel CSS */
    body::-webkit-scrollbar {
        width: 10px;
    }

    body::-webkit-scrollbar-track {
        background: #f1f1f1;
        border-radius: 10px;
        box-shadow: inset 0 0 5px grey;
        opacity: 0.5;
    }
    
    body::-webkit-scrollbar-thumb {
        background: #888;
        border-radius: 10px; 
    }

    body::-webkit-scrollbar-thumb:hover {
        background: #555;
    }
    
    /* General CSS */
    body{
        height: 100vh;
        background-color: #000;
        background-image: url($lib/images/bg2.jpg);
        background-size: cover;
        background-repeat: repeat;
        background-position: center;
        background-attachment: fixed;
        font-size: 20px;
    }

    section {
        padding: 5vh;
        margin-top: 2vh;
        margin-bottom: 2vh;
        border-radius: 25px;
    }

    div{
        padding: 3vh;
        margin: 1vh;
        border-radius: 25px;
        text-align: justify;
    }

    /* Specific CSS */
    .content{
        margin-top: 70px;
        margin-bottom: 0;
        padding: 0;
        position: static;
    }

    #sub {
        padding: 2em;
        margin: 2vh;
        border-radius: 20px;
        background-color: rgb(99,132,173,0.6);
        text-align: justify;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    #sub1 {
        padding: 1em;
        margin: 1vh;
        border-radius: 20px;
        background-color: rgb(99,132,173,0.6);
        text-align: justify;
    }
    
    #sub2 {
        padding: 1em;
        margin-top: 3vh;
        margin-bottom: 3vh;
        border-radius: 20px;
        background-color: rgb(99,132,173,0.5);
        text-align: justify;
    }

    #sub3 {
        padding: 1em;
        border-radius: 20px;
        background-color: rgb(99,132,173,0.5);
        text-align: justify;
    }

    #sub4 {
        padding: 20px;
        margin: 1vh;
        border-radius: 20px;
        background-color: rgb(27,24,28,0.8);
        text-align: justify;
    }
    
    #quote {
        font-size: 50px;
        text-align: center;
        position: relative;
        padding: 0 40px;
        &::before{
            content: "\201C";
            position: absolute;
            font-weight: bold;
            font-size: 3em;
            top: -0.3em;
            left: -1vw;
        }
        &::after{
            content: "\201D";
            position: absolute;
            font-weight: bold;
            font-size: 3em;
            bottom: -0.5em;
            right: -1vw;
        }
    }

    #DataRepo{
        background-color: rgb(209, 209, 209, 0.9);
        border-radius: 0;
    }

    #DataRepo h1{
        color: #03042d;
    }

    /* Navbar CSS */
    .navbar{
        top: 0;
        margin: 0;
        padding: 10px;
        width: 100%;
        height: 70px;
        background-color: rgb(63, 66, 69);
        position: fixed;
        display: flex;
        align-items: center;
        overflow: hidden;
        z-index: 1;
    }

    .navbar a{
        float: left;
        padding: auto;
        color: white;
        text-align: center;
        padding: 1vw;
        text-decoration: none;
    }

    .navbar #sussy{
        border-right-style: solid;
    }

    .navbar #sussy:hover{
        background-color: white;
        transition: 0.6s;
        color: #03042d;
    }

    .navbar a:hover{
        background-color: #03042d;
        color: white;
        transition: 0.4s;
    }
    
    /* Grid-based CSS */

    .wrapper{
        display: grid;
        padding: 5vw 5vh;
        grid-template-columns: 1fr 1fr;
    }

    .wrapper2{
        display: grid;
        grid-template-columns: 1fr 1fr;
        width: 100%;
    }

    .wrapper3{
        display: grid;
        padding: 0;
        grid-template-columns: 1fr 1fr 1fr;
    }

    .wrapper4{
        display: grid;
        grid-template-columns: 1fr 3fr;
        padding-left: 0;
        padding-right: 0;
    }

    .box1{
        grid-column-start: 1;
        grid-column-end: 2;
        grid-row-start: 1;
        grid-row-end: 2;
        background-color: rgb(99,132,173,0.3);
    }

    .box2{
        grid-column-start: 1;
        grid-column-end: 2;
        grid-row-start: 2;
        grid-row-end: 3;
        background-color: rgb(99,132,173,0.3);
    }

    .box3{
        grid-column-start: 2;
        grid-column-end: 3;
        grid-row-start: 1;
        grid-row-end: 3;
        background-color: rgb(99,132,173,0.3);
    }

    .box11{
        grid-column-start: 1;
        grid-column-end: 2;
        grid-row-start: 2;
        grid-row-end: 3;
        background-color: rgb(99,132,173,0.3);
    }

    .box12{
        grid-column-start: 2;
        grid-column-end: 3;
        grid-row-start: 2;
        grid-row-end: 3;
        background-color: rgb(99,132,173,0.3);
    }

    .about1{
        grid-column-start: 1;
        grid-column-end: 2;
        background-color: rgb(99,132,173,0.3);
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    }
    .about2{
        grid-column-start: 2;
        grid-column-end: 3;
        background-color: rgb(99,132,173,0.3);
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    }
    .about3{
        grid-column-start: 3;
        grid-column-end: 4;
        background-color: rgb(99,132,173,0.3);
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    }

    .intro2{
        grid-column-start: 2;
        grid-column-end: 4;
    }

    .image{
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-wrap: wrap;
        grid-column-start: 1;
        grid-column-end: 2;
    }
    
    /* Miscellaneous */
    .center {
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 100%;
    }

    a {
        color: #03042d;
    }

    li {
        font-size: 20px;
    }

    ul {
        padding-left: 30px;
    }

    p {
        font-size: 20px
    }
</style>
