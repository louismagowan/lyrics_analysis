<div id="top"></div>
<!--
*** Copied from https://github.com/othneildrew/Best-README-Template/blob/master/BLANK_README.md
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<h3 align="center">Song Lyrics Over Time: Lexical Diversity and Sentiment Analysis in R</h3>

  <p align="center">
    Using Quanteda, IBM Tone Analyzer and ggplot2 to analyse top 100 song lyrics in the US from 1958.
    <br />
    <br />
    <a href="https://datastudio.google.com/reporting/428bdb5c-8375-4566-a013-e8f7a3821256">Data Studio Dashboard</a>
    ·
    <a href="https://github.com/louismagowan/lyrics_analysis/issues">Request Feature</a>
    ·
    <a href="https://github.com/louismagowan/lyrics_analysis/issues">Report Bug</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

Uses lyrics from [Billboard Top 100 songs](https://www.kaggle.com/dhruvildave/billboard-the-hot-100-songs) from 1958 in the US to do sentiment and lexical diversity analysis. 
Aims to determine if/how song lyrics have changed over time. Lexical diversity analysis is conducted using the Quanteda package, 
with the [TTR](https://rdrr.io/cran/koRpus/man/TTR.html) and [Maas](https://rdrr.io/cran/koRpus/man/maas.html) measures.

Sentiment analysis run using [IBM's tone analyser](https://www.ibm.com/uk-en/cloud/watson-tone-analyzer).

Songs appear to have become less joyful, angrier and simpler.

To analyse / play about with the data yourself, please check out the [Data Studio dashboard](https://datastudio.google.com/reporting/428bdb5c-8375-4566-a013-e8f7a3821256).

<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

* [Quanteda](https://quanteda.io/index.html)
* [Data Studio](https://datastudio.google.com/reporting/428bdb5c-8375-4566-a013-e8f7a3821256)
* [plotly](https://plotly.com/r/)
* [httr](https://cran.r-project.org/web/packages/httr/vignettes/quickstart.html)
* [IBM Tone Analyzer](https://www.ibm.com/uk-en/cloud/watson-tone-analyzer)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

Make sure you've done this setup before you try to run the code yourself.

### Prerequisites

Install Quanteda packages in R environment.
* R
  ```r
  install.packages("quanteda")
  install.packages("quanteda.textstats")
  install.packages("quanteda.textmodels")
  ```

* IBM Cloud Account
  Create a free IBM Cloud Account and use the $200 USD credit they give you to create a Tone Analyzer instance,
  if you want to run the sentiment analysis yourself. [IBM Tone Analyzer](https://www.ibm.com/uk-en/cloud/watson-tone-analyzer)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [ ] Genre-level analysis
- [ ] Analysis of more songs, top 100 in other countries
    - [ ] Country-level comparison


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

LinkedIn- [Louis Magowan](https://www.linkedin.com/in/louismagowan/)

Project Link: [https://github.com/louismagowan/lyrics_analysis](https://github.com/louismagowan/lyrics_analysis)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [othneildrew - README template](https://github.com/othneildrew/Best-README-Template/blob/master/BLANK_README.md)
* [Group By Decade](https://stackoverflow.com/questions/47799182/grouping-data-in-r-and-summing-by-decade)
* [Lyrics API](https://api.lyrics.ovh/v1/)
* [Dhruvil Dave, Billboard Top 100 Songs](https://www.kaggle.com/dhruvildave/billboard-the-hot-100-songs)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/louismagowan/lyrics_analysis.svg?style=for-the-badge
[contributors-url]: https://github.com/louismagowan/lyrics_analysis/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/louismagowan/lyrics_analysis.svg?style=for-the-badge
[forks-url]: https://github.com/louismagowan/lyrics_analysis/network/members
[stars-shield]: https://img.shields.io/github/stars/louismagowan/lyrics_analysis.svg?style=for-the-badge
[stars-url]: https://github.com/louismagowan/lyrics_analysis/stargazers
[issues-shield]: https://img.shields.io/github/issues/louismagowan/lyrics_analysis.svg?style=for-the-badge
[issues-url]: https://github.com/louismagowan/lyrics_analysis/issues
[license-shield]: https://img.shields.io/github/license/louismagowan/lyrics_analysis.svg?style=for-the-badge
[license-url]: https://github.com/louismagowan/lyrics_analysis/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/louismagowan/
[product-screenshot]: images/screenshot.png