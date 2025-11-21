library(shiny)
library(bslib)
library(shinythemes)
library(shinyWidgets)


link_pricing <- tags$a(
  shiny::icon("file"), "U.S. House of Representatives Drug Pricing Investigation 2021", 
  href = "https://oversightdemocrats.house.gov/sites/evo-subsites/democrats-oversight.house.gov/files/DRUG%20PRICING%20REPORT%20WITH%20APPENDIX%20v3.pdf"
)

ui <- page_navbar(
  title = tags$div(img(src = "Manungal_logo.png", height = "80px"), 
          tags$b("Yudi Inc."),
            style = "color:white;
                     font-size: 30px;",
            font = font_google("Nunito Sans"),
  ),
  nav_spacer(),
  theme = bs_theme(preset = "lux",bg = "#101010",fg = "#FFF"),
  nav_panel(
    title = "Home",
    tags$head(
      tags$style(HTML("
      .title-text {
        position: absolute;
        top: 15%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white; /* Adjust text color as needed */
        font-size: 24px; /* Adjust font size as needed */
        text-align: center;
        width: 100%; /* Ensure text takes full width of its container */
      }
      .lower-text {
        position: absolute;
        top: 23%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white; /* Adjust text color as needed */
        font-size: 24px; /* Adjust font size as needed */
        text-align: center;
        width: 100%; /* Ensure text takes full width of its container */
      }
      .trademark-text {
        position: absolute;
        top: 11%;
        left: 56.5%;
        transform: translate(-50%, -50%);
        color: white; /* Adjust text color as needed */
        font-size: 24px; /* Adjust font size as needed */
        text-align: center;
        width: 100%; /* Ensure text takes full width of its container */
      }
    "))
    ),
    div(
      style = "position: relative; width: 100%; height: 100%; overflow: hidden;", 
      img(
        src = 'HomePage.png',
        style = "width: 100%; height: 100%; object-fit: cover;"
      ),
      absolutePanel(
        class = "title-text",
        h2(
          p(tags$b("LIFE"),
             style = "color:white;
                      font-size: 100px;",
                            
             font = font_google("Nunito Sans")
            )
          )
      ),
      absolutePanel(
        class = "trademark-text",
        p(tags$b("®"),
          style = "color:white;
                   font-size: 20px;",
          font = font_google("Nunito Sans")
        )
      ),
      absolutePanel(
        class = "lower-text",
        h2(
          p(tags$b("*Starting at 2,500$ for a 1 month supply"),
            style = "color:white;
                             font-size: 20px;
                             font-stretch: 100%;
                             font-weight:100;",
            font = font_google("Nunito Sans")
          )
        ) 
      )
    )
  ),
  nav_panel(
    title = "About Us",
    absolutePanel(
      width = '100%',
      img(
        src = 'AboutUS2.png',
        width = "100%",
        height = "100%",
        top = '10%',
        style = "object-fit: cover;")
    ),
    absolutePanel(
      width = '20%',
      height = '20%',
      top = '12.5%',
      tags$b("OUR MISSION"),
      style = "color:white;
               font-size: 50px;
               font-stretch: 100%;
               font-weight: 1000;",
      font = font_google("Nunito Sans"),
      
    ),
    absolutePanel(
      width = '20%',
      top = '20%',
      height = '80%',
      tags$b("When you’re living with a disease, all you want is to feel relief. To feel improvement. To feel healthy. As a medicine company that believes health is fundamental to our lives, those are the people we’re working for. The people who are counting on a breakthrough, desperately waiting for science to catch up. We beleive it is our duty to fight for our patients until the day their bank accounts run dry."),
      style = "color:white;
               font-size: 20px;
               font-stretch: 100%;
               font-weight: 1000;
               backdrop-filter: blur(8px);",
      font = font_google("Nunito Sans")
    )
  ),
  nav_panel(
    title = "Patients",
    absolutePanel(
      width = '20%',
      top = '12.5%',
      tags$b("HEAR FROM OUR PATIENTS"),
      style = "color:white;
               font-size: 50px;
               font-stretch: 100%;
               font-weight: 1000;",
      font = font_google("Nunito Sans")
    ),
    absolutePanel(
      width = '20%',
      top = '35%',
      tags$b(HTML("We know that many people are skeptical of the pharmaceutical industry, so we'll let our real customers tell you about their experience with LIFE<sup><small><small>®</small></small></sup>")),
      style = "color:white;
               font-size: 20px;",
      font = font_google("Nunito Sans")
    ),
    absolutePanel(
      width = '90%',
      left = '25%',
      top = '13.6%',
      tags$style("#project-grid2 {
                      display: grid;
                      grid-template-rows: 10px
                      grid-gap: 10px;
                      }"
      ),
      div(id = "project-grid2",
          div(
            div(img(src = 'Patient2.png', width = '1100px')),
            div(h4('Patient A'),
                p(tags$b(HTML("Patient A died less than one month after going off of his mother's insurance. His family thinks he was rationing his LIFE<sup><small><small>®</small></small></sup> — using less than he needed — <br> to try to make it last until he could afford to buy more. He died alone in his apartment three days before payday. The LIFE<sup><small><small>®</small></small></sup> pen he used to give himself shots was empty.")),
                  style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                  font = font_google("Nunito Sans")))),
          div(
            div(img(src = 'Patient1.png', width = '1100px')),
            div(h4('Patient B'),
                p(tags$b(HTML("When they lost their job and insurance, Patient B struggled to afford LIFE<sup><small><small>®</small></small></sup> which cost more than $800 a month. They resorted to buying <br> NPH LIFE<sup><small><small>®</small></small></sup> from Walmart, which is cheaper but much more unpredictable than the original LIFE<sup><small><small>®</small></small></sup> formula. On Christmas Day, 2018, Patient B died due to <br> LIFE<sup><small><small>®</small></small></sup> rationing, one day before they would have received a paycheck that could have paid for their prescription.")),
                  style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                  font = font_google("Nunito Sans")))))
      )
  ),
  nav_panel(title = "Leadership",
          absolutePanel(
            width = '100%',
            img(
              src = 'tst3.png',
              width = "100%",
              height = "90%",
              top = '10%',
              style = "object-fit: cover; filter: blur(4px);")
            ),
          absolutePanel(
            left= '15px',
            top = '10%',
            width = '20%',
            height = '110%',
            absolutePanel(
              left= '20px',
              top = '1.5%',
              p(tags$b("MEET OUR EXECUTIVE TEAM"),
                    style = "color:white;
                             font-size: 50px;
                             font-stretch: 100%;
                             font-weight: 1000;",
                    font = font_google("Nunito Sans")
               )
            ),
            style = "backdrop-filter: blur(8px);"
          ),
          absolutePanel(
                   top = '13%',
                   left = '25%',
                   tags$style("#project-grid {
                      display: grid;
                      grid-template-columns: 300px 300px 300px 300px;
                      grid-gap: 10px;
                      }"
                    ),
                   div(id = "project-grid",
                       div(
                         div(img(src = 'Lars_Jorgensen.png', style = 'border-radius: 10%', width = '200px')),
                         div(h4('Lars Jorgensen'),
                             p(tags$b(HTML("Lars Jorgensen knew that the vast majority of the projected growth for LIFE<sup><small><small>®</small></small></sup> would come from price appreciation as opposed to volume growth. He argued that price increases reflected the need to dig out of the hole created by the significant loss of returning patients.")),
                               style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                               font = font_google("Nunito Sans")))),
                       div(
                         div(img(src = 'Paul_Hudson.png', style = 'border-radius: 10%', width = '200px')),
                         div(h4('Paul Hudson'),
                             p(tags$b(HTML("Paul Hudsons 2019 compensation plan tied bonus payments to net revenue and pre-tax income targets, accounting for as much as 80% of his bonus calculation. Yudi had a net revenue of $33.3 billion that year, achieving 101% of its target. Without raising the prices of LIFE<sup><small><small>®</small></small></sup> by 12% in 2019, the Committee estimates that Yudi would have missed this target. Because Yudi met its income and revenue targets, Paul Hudson was paid $70 million in 2019.")),
                               style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                               font = font_google("Nunito Sans")))),
                       div(
                         div(img(src = 'Mark_Trdeau.png', style = 'border-radius: 10%', width = '200px')),
                         div(h4('Mark Trdeau'),
                             p(tags$b(HTML("Mark Trdeau helped developed the new formulation of LIFE<sup><small><small>®</small></small></sup> in part in an attempt to extend its monopoly pricing by shifting patients to the new controlled-release formulation—which still enjoyed market exclusivity—before he anticipated LIFE<sup><small><small>®</small></small></sup>’s original formulation would begin facing generic competition.")),
                               style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                               font = font_google("Nunito Sans")))),
                       div(
                         div(img(src = 'Vas_Narasimhan.png', style = 'border-radius: 10%', width = '200px')),
                         div(h4('Vas Narasimhan'),
                             p(tags$b(HTML("Vas Narasimhan helped abuse the Orphan Drug Act, which is intended to incentivize the development of drugs that treat rare diseases. By leveraging the orphan drug designation as a justification for the high price of LIFE<sup><small><small>®</small></small></sup>, he helped aggressively expand sales to non-orphan indications at the same high price, with the objective of bringing in top-level shareholder returns.")),
                               style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                               font = font_google("Nunito Sans")))),
                       div(
                         div(img(src = 'Robert_Bradway.png', style = 'border-radius: 10%', width = '200px')),
                         div(h4('Robert Bradway'),
                             p(tags$b(HTML("Robert Bradway is routinely contacted by patients who cannot afford their medications. He is aware of the impact price increases are having on patients. He has read hundreds of pages of patient complaints describing how the the high price of LIFE<sup><small><small>®</small></small></sup> has impacted their lives and their loved ones.")),
                               style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                               font = font_google("Nunito Sans")))),
                       div(
                       div(img(src = 'Albert_Bouria.png', style = 'border-radius: 10%', width = '200px')),
                       div(h4('Albert Bouria'),
                           p(tags$b(HTML("Albert Bouria has helped issue almost 500 patents, collectively providing more than 200 years of potential market monopolies on LIFE<sup><small><small>®</small></small></sup>")),
                           style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                           font = font_google("Nunito Sans")))),
                       div(
                       div(img(src = 'Dave_Ricks.png', style = 'border-radius: 10%', width = '200px')),
                       div(h4('Dave Ricks'),
                           p(tags$b(HTML("Dave Ricks has received more than $500,000 in bonus payments in 2016 and 2017 solely attributable to the Yudi's price increases for the cancer drug LIFE<sup><small><small>®</small></small></sup>")),
                             style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                             font = font_google("Nunito Sans")))),
                       div(
                       div(img(src = 'Kare_Schultz.png', style = 'border-radius: 10%', width = '200px')),
                       div(h4('Kare Schultz'),
                           p(tags$b(HTML("Kare Schultz has helped increase the price of LIFE<sup><small><small>®</small></small></sup> by over 100,000% since its launch, with a net profit in excess of 39,000$ per vial.")),
                             style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;",
                             font = font_google("Nunito Sans"))))
                       # div(
                       # div(img(src = 'Mark_Alles.png', style = 'border-radius: 10%', width = '200px')),
                       # div(h4('Mark Alles'),
                       #     p(tags$b("Mark Alles was able to combat generic competition by launching a daily dose of LIFE<sup><small><small>®</small></small></sup>. Despite the failure of clinical trials and the objections of Manungals scientists, he shifted the company’s strategy to promoting LIFE<sup><small><small>®</small></small></sup> 40 mg/mL as an equally effective but less frequent dose, costing the U.S. health care system between $4.3 billion and $6.5 billion in additional health care expenditures between 2015 and 2017 due to delayed generic competition related to the introduction of the new version of the drug."),
                       #       style = "color:white;
                       #       font-size: 15px;
                       #       font-stretch: 100%;
                       #       font-weight:100;",
                       #       font = font_google("Nunito Sans")))),
                       # div(
                       # div(img(src = 'Richard_Gonzalez.png', style = 'border-radius: 10%', width = '200px')),
                       # div(h4('Richard Gonzalez'),
                       #     p(tags$b("Richard Gonzalez was paid $170 million between 2013 and 2020, as Yudiraised the price of LIFE<sup><small><small>®</small></small></sup> 14 times from approximately $1,000 per syringe to nearly $3,000 per syringe"),
                       #       style = "color:white;
                       #       font-size: 15px;
                       #       font-stretch: 100%;
                       #       font-weight:100;",
                       #       font = font_google("Nunito Sans")))),
                   )
          )
  ),
  nav_panel(
    title = "Order Now",
    tags$head(
      tags$style(HTML("
      .title-text {
        position: absolute;
        top: 15%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white; /* Adjust text color as needed */
        text-align: center;
        width: 100%; /* Ensure text takes full width of its container */
      }
      .lower-text {
        position: absolute;
        top: 23%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white; /* Adjust text color as needed */
        font-size: 24px; /* Adjust font size as needed */
        text-align: center;
        width: 100%; /* Ensure text takes full width of its container */
      }
      .order-text {
        position: absolute;
        top: 26%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white; /* Adjust text color as needed */
        text-align: center;
        width: 100%; /* Ensure text takes full width of its container */
      }
    "))
    ),
    div(
      style = "position: relative; width: 100%; height: 100%; overflow: hidden;", 
      img(
        src = 'OneWeekLeft.png',
        width = '95%',
        height = '100%',
        style = "width: 100%; height: 100%; object-fit: cover;"
      ),
      absolutePanel(
        class = "title-text",
        h2(
          p(tags$b("One week left"),
            style = "color:white;
                             font-size: 100px;
                             font-stretch: 800%;
                             font-weight: 1000;
                             text-shadow: 1px 2px 4px rgba(0, 0, 0, 1);",
            font = font_google("Nunito Sans")
          )
        )
      ),
      absolutePanel(
        class = "lower-text",
        h2(
          p(tags$b("Can you afford another month?"),
            style = "color:white;
                             font-size: 20px;
                             font-stretch: 100%;
                             font-weight:100;",
            font = font_google("Nunito Sans")
          )
        ) 
      ),
      absolutePanel(
        class = "order-text",
        h2(
          p(tags$b("Order Now"),
            style = "color:white;
                             font-size: 15px;
                             font-stretch: 100%;
                             font-weight:100;
                             text-decoration: underline;",
            font = font_google("Nunito Sans")
          )
        ) 
      )
    )
  ),
  nav_panel(
    title= 'tst',
    absolutePanel(
      width= '100%',
      height = '100%',
      tags$iframe(
        src = "https://cosmograph.app/run/?data=www/main_dat.csv", # Relative path from the 'www' folder
        width = "100%",
        height = "100%"
      )
    )
  ),
  nav_spacer(),
  nav_menu(
    title = "Links",
    align = "right",
    nav_item(link_pricing)
  )
)

server <- function(input, output) {}
shinyApp(ui = ui, server = server)