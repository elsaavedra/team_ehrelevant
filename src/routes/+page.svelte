<body>
    <h1>Welcome to SvelteKit</h1>
    <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

    <marquee scrollamount=20> hello world </marquee>

    <section>
        <h1> Background of the Study </h1>
            <p> 
                According to John Dewey, “Education is not preparation for life; education is life itself.”
                Truly, it is quite evident that one's education strongly influences the kind of life that one lives.
                Various reasons one may have to further their education, whether it is to apply for practical knowledge or deepen their understanding in specialized fields, but one thing remains the same; education.
                However, one's education, strictly focusing on the schooling aspect of education, isn't necessarily applicable to one's field of work.
                This may be due to many reasons such as a shift in interest, a cruel demand in one's specialization, or simply the lack of available jobs.
            </p>

            <p>
                In the Philippines, one such shift in education would be the implementation of the K-12 basic education curriculum in 2012.
                This change was an attempt to improve current schooling to bring up “job-ready” students after graduating their 12th grade.
                Despite the improvement in their Math and Science subjects, most major companies in the Philippines would still prefer college graduates over high school graduates.<sup><a href="https://www.philstar.com/headlines/2023/05/12/2265854/deped-forms-task-force-employability-issues-senior-high-graduates">[1]</a></sup>
                Most K-12 graduates that were lucky enough to be employed receive only minimum wage for entry-level positions while college graduates receive many more benefits than this.<sup><a href="https://www.philstar.com/headlines/2023/12/04/2316419/most-job-vacancies-accepting-senior-high-grads-offer-minimum-wage-work-dole">[2]</a></sup>
                This heavily contrasts one of the main objectives of K-12 to “produce employable students as early as post-high school”. <sup><a href="https://www.philstar.com/headlines/2023/05/12/2265854/deped-forms-task-force-employability-issues-senior-high-graduates">[3]</a></sup>
            </p>
    </section>

    <section>
        <h2> Problem </h2>
            <p>
                Graduates in the Philippines, specifically senior high school graduates of the
                K-12 basic education,are being discriminated against in terms of employment.
            </p>
    </section>

    <section>
        <h2> Solution </h2>
            <p>
                The goal of this research is to use data science to analyze the actual importance
                of knowledge gained in school across different fields and possible benchmarks
                for useful knowledge, in turn finding practical solutions to employ K-12 graduates.
            </p>
    </section>

    <section>
        <h2> Objectives </h2>
            <p>
                In addition, the research aims to answer the following questions:
            </p>

            <ul>
                <li>Does the level of participation of Filipinos in different fields of expertise correlate with their highest level of educational attainment?</li>
                <li>Across different fields of expertise, how useful is knowledge learned from school to Filipinos seeking jobs?</li>
            </ul>
    </section>

    <section>
        <h2> Hypotheses </h2>
            <h3> Null Hypothesis </h3>
                <p>
                    There is no correlation between the level of participation of Filipinos
                    in different fields of expertise and their highest level of education
                    nor the usefulness of their knowledge learned from school.
                </p>

            <h3> Alternative Hypothesis </h3>
                <p>
                    The level of participation of Filipinos in different fields of expertise
                    influences the perceived usefulness of knowledge learned from school,
                    or varies among Filipinos with different highest levels of education attained.
                </p>
    </section>

    <section>
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

        <section id="sub">
        <h2> Dataset Link </h2>
            <a href="https://docs.google.com/spreadsheets/d/1wG50_tLEtZrU1jB0AkM7doo6a6njIig8xorNHGk05Ig/edit#gid=1228805475">Here</a> is a link to the datasheet that will be used for this research. This contains the following:
            
            <ul>
                <li>Selected questions from FLEMMS 2019 dataset to be analyzed</li>
                <li>Dictionary of selected questions from FLEMMS 2019 dataset to be analyzed</li>
                <li>Full unedited FLEMMS 2019 dataset</li>
                <li>Dictionary of the unedited FLEMMS 2019 dataset</li>
            </ul>
        </section>
    </section>
</body>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body::-webkit-scrollbar {
            display: none;
        }

        body{
            height: 100vh;
            background-color: #000;
            background-image: url($lib/images/bg.jpg);
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }

        section {
            padding: 10px;
            margin-top: 5vh;
            margin-bottom: 5vh;
            border-radius: 25px;
            background-color: rgb(52, 115, 232);
        }

        #sub {
            padding: 10px;
            margin-top: 5vh;
            margin-bottom: 5vh;
            border-radius: 25px;
            background-color: rgb(174, 180, 193);
        }

        li {
            list-style: none;
        }
    </style>
