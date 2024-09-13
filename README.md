# Continuous Deployment Game that uses AWS Code Pipeline and Amazon S3

## TL;DR
The game's code is stored in GitHub. We set up an S3 bucket for static website hosting and configure a continuous deployment pipeline with AWS CodePipeline to automatically deploy updates whenever changes are made to the code.

## The Game
A basic memory matching game where the user selects two cards, each displaying a metallica band member's image, in an attempt to find a match. If the cards match, they are removed from the board. If not, the cards flip back to the Metallica Card sides, allowing the user to try again.

The game consists of HTML, CSS and JavaScript.

Ideas for additional features:
- Fun facts about the members after a successful match
- Method of keeping score
- Expand to include more bands
- A timer

## The Deployment Environment
The code will be deployed and hosted in S3.

## The Deployment Pipeline
The pipeline is built with AWS CodePipeline. It retrieves the code from GitHub and deploys it to S3 whenever changes in the code are detected.

## Cost
All services used are covered by the [AWS Free Tier](https://aws.amazon.com/free/), but charges may apply after a certain usage limit. It is advised to shut down resources once you finish the tutorial to avoid any unexpected costs.