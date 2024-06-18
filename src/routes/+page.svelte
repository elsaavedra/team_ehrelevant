<script>
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
        <a href="#Model">Modelling</a>
        <a href="#Conc">Conclusion</a>
    </ul>
    
    <div class="content">
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

        <p id="sub">
            In the Philippines, one such shift in education would be the implementation of the K-12 basic education curriculum in 2012.
            This change was an attempt to improve current schooling to bring up “job-ready” students after graduating their 12th grade.
            Despite the improvement in their Math and Science subjects, most major companies in the Philippines would still prefer college graduates over high school graduates.<sup><a href="https://www.philstar.com/headlines/2023/05/12/2265854/deped-forms-task-force-employability-issues-senior-high-graduates">[1]</a></sup>
            Most K-12 graduates that were lucky enough to be employed receive only minimum wage for entry-level positions while college graduates receive many more benefits than this.<sup><a href="https://www.philstar.com/headlines/2023/12/04/2316419/most-job-vacancies-accepting-senior-high-grads-offer-minimum-wage-work-dole">[2]</a></sup>
            This heavily contrasts one of the main objectives of K-12 to “produce employable students as early as post-high school”. <sup><a href="https://www.philstar.com/headlines/2023/05/12/2265854/deped-forms-task-force-employability-issues-senior-high-graduates">[3]</a></sup>
        </p>
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
                        Across different fields of expertise, the perceived usefulness of knowledge learned from school does not influence Filipinos seeking jobs.
                    </p>

                <h3> Alternative Hypothesis </h3>
                    <p id="sub2">
                        Across different fields of expertise, the perceived usefulness of knowledge learned from school influences Filipinos seeking jobs.
                    </p>
        </div>

    </section>

    <section id="DataRepo">
    <h1> Dataset Description </h1>
        <section id="sub">
            <h2> Dataset Source: FLEMMS 2019 </h2>
                <p>
                    The Philippine Statistics Authority (PSA) organizes a survey known as the <a href = "https://psada.psa.gov.ph/catalog/FLEMMS/about"> Functional Literacy, Education and Mass Media Survey (FLEMMS) </a> as a regular check on the state of the country's education systems.
                    FLEMMS collects general information about each respondent's educational background, demographic information, and household information, followed by questions to ask and assess their ability to read, write, and answer questions.
                    These assessments are then interpreted to classify each respondent's educational skills through a metric known as the Functional Literacy [Level].

                    As of April 2024, the most updated results available for the FLEMMS survey are those from the FLEMMS 2019 survey, whose report may be found through <a href="https://lcc.deped.gov.ph/ls-flemms/"> this link </a>.
                </p>
        </section>

        <section id="sub">
            <h2> Data Collection </h2>
                <p> 
                    The results of the FLEMMS 2019 survey are divided into several CSV (Comma Separated Value) files tabulating the information gathered from each respondent.
                    Among the files, this study intends to investigate the data from the responses in the Household Name CSV file. The Household Name CSV contains the respondents' answers to the Individual Questionnaire, which contains questions that directly assess their educational background and overall literacy.
                    The relevant files for the FLEMMS 2019 dataset can be downloaded from the <a href="https://psada.psa.gov.ph/catalog/FLEMMS/about"> Philippine Statistics Authority Data Archive (PSADA) website </a>.
                </p>
        </section>

        <section id="sub">
            <h2> Data Preprocessing </h2>
                <p> 
                    From the Household Name CSV, the first few fields are kept to uniquely identify each of the data points of the dataset, namely the Region (REG), Urbanity (URB), Household ID (HHID), and the Respondent Line Number (RESP_LNO).
                </p>

                <p> 
                    Furthermore, certain fields were found to be the most relevant to the study as variables to be kept, namely the Level of Participation (Q15A_ARTS, Q15B_SCIENCE, Q15C_BUSINESS), Knowledge in Job (Q21_KNOWLEDGE), and Highest Educational Attainment (C12_HEA_RT04).
                    Other than these, other “potentially useful” fields were also kept for possible sub-correlation or confounding variables, which include the Technical-Vocational Variables (Q5_TECHVOC, Q5_TECHVOC_COURSE, Q5_SPECIFY_COURSE), the TESDA National Certification (Q6_TESDA_CERT),
                    Activities to help other people (Q20_ACTIVITY), Age (C5_AGE_RT04), Sex (C4_SEX_RT04), and Ongoing School Status (C14_ATTEND_SCHOOL_RT04).
                </p>

                <p> 
                    As such, the above-mentioned variables are kept in the “specific variables” to be used for the study, with any other columns deleted from the dataset. Nonetheless, both this reduced dataset and the full dataset may be found in the link below, for viewing reference.
                </p>
        </section>

        <section id="sub1">
        <h2> Dataset Link </h2>
            <p><a href="https://docs.google.com/spreadsheets/d/1wG50_tLEtZrU1jB0AkM7doo6a6njIig8xorNHGk05Ig/edit#gid=1228805475">Here</a> is a link to the datasheet that will be used for this research. This contains the following: </p>
            
            <ul id="sub3">
                <li>Selected questions from FLEMMS 2019 dataset to be analyzed</li>
                <li>Dictionary of selected questions from FLEMMS 2019 dataset to be analyzed</li>
                <li>Full unedited FLEMMS 2019 dataset</li>
                <li>Dictionary of the unedited FLEMMS 2019 dataset</li>
            </ul>
        </section>
    </section>

    <section id="DataVisual">
        <h1> Visualization of Data </h1>
        <section class="wrapper3">
            <section id="sub">
                <img src={a1} alt="Participation in Arts" width=50% class="center">
                <p style="text-align:center">Level of Participation in Arts vs Highest Educational Attainment</p>
            </section>
            <section id="sub">
                <img src={b1} alt="Participation in Science" width=50% class="center">
                <p style="text-align:center">Level of Participation in Science vs Highest Educational Attainment</p>
            </section>
            <section id="sub">
                <img src={c1} alt="Participation in Business" width=50% class="center">
                <p style="text-align:center">Level of Participation in Business vs Highest Educational Attainment</p>
            </section>
        </section>

        <section class="wrapper3">
            <section id="sub">
                <img src={a2} alt="Knowledge in Arts" class="center">
                <p style="text-align:center">Perceived Use of Knowledge vs Level of Participation in Arts</p>
            </section>
            <section id="sub">
                <img src={b2} alt="Knowledge in Science" class="center">
                <p style="text-align:center">Perceived Use of Knowledge vs Level of Participation in Science</p>
            </section>
            <section id="sub">
                <img src={c2} alt="Knowledge in Business" class="center">
                <p style="text-align:center">Perceived Use of Knowledge vs Level of Participation in Business</p>
            </section>
        </section>
    </section>

    <section>
        <h1> Hypothesis Testing </h1>
        <section id="sub">
            <img src={hyp} alt="Hypothesis Testing" class="center" style='width: 50%'>
            <p style="text-align:center">Significance of First Hypothesis</p>
        </section>
    </section>

    <section id="Model">
        <h1> Modelling </h1>
        <section id="sub">
            <p style="text-align:center">Lorem Ipsum</p>
        </section>
    </section>

    <section id="Conc">
        <h1> Conclusion </h1>
        <section id="sub">
            <p style="text-align:center">Lorem Ipsum</p>
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
                    Good morning there! I am Lawrence, a 2nd year Computer Science student at UP Diliman. I enjoy programming casually, whether for games or for just appreciating the logic with how programs work <br> <br>
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
                    I also enjoy watching vtubers in my spare time (go watch <a href="https://www.youtube.com/@TakaneLui">Takane Lui</a>)
                </p>
                <p style="text-align:center"> <br> <br> <br> elsaavedra@up.edu.ph</p>
            </div>
        </section>
    </section>
    </div>
</body>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
            color: #FFF;
        }

        body::-webkit-scrollbar {
            display: none;
        }

        body{
            height: 100vh;
            background-color: #000;
            background-image: url($lib/images/bg2.jpg);
            background-size: cover;
            background-repeat: repeat;
            background-position: center;
            background-attachment: fixed;
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

        .content{
            margin-top: 50px;
            margin-bottom: 0;
            position: static;
        }

        #sub {
            padding: 2em;
            margin: 2vh;
            border-radius: 20px;
            background-color: rgb(99,132,173,0.7);
            text-align: justify;
        }

        #sub1 {
            padding: 5em;
            margin-top: 3vh;
            margin-bottom: 3vh;
            border-radius: 20px;
            background-color: rgb(99,132,173,0.3);
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

        .navbar{
            top: 0;
            margin: 0;
            padding: 10px;
            width: 100%;
            background-color: rgb(93,100,106);
            height: auto;
            position: fixed;
            overflow: hidden;
            z-index: 1;
        }

        .navbar a{
            float: left;
            padding: auto;
            font-size: 20px;
            color: white;
            text-align: center;
            padding: 1vw;
            text-decoration: none;
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

        .wrapper3{
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
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
            list-style: none;
            font-size: 20px
        }

        p {
            font-size: 20px
        }
    </style>
