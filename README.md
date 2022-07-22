<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
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
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/C5H8NNaO4/tarent-challenge">
    <img src="https://www.tarent.de/wp-content/uploads/dark.svg" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Tarent Coding Challenge</h3>

  <p align="center">
    A small SPA to showcase basic react / fullstack skill.
    <br />
    <a href="https://github.com/C5H8NNaO4/tarent-challenge"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/C5H8NNaO4/tarent-challenge">View Demo</a>
    ·
    <a href="https://github.com/C5H8NNaO4/tarent-challenge/issues">Report Bug</a>
    ·
    <a href="https://github.com/C5H8NNaO4/tarent-challenge/issues">Request Feature</a>
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
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](http://localhost:3000)

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With
* Love
* [React.js](https://reactjs.org/)
* [express](https://expressjs.com/)
* [Swagger](https://swagger.io/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Clone the repo
   ```sh
   git clone --recurse-submodules -j2 https://github.com/C5H8NNaO4/tarent-challenge.git
   ```
3. Open a split terminal and install NPM packages for both, frontend and backend repo.
   ```sh
   cd tarent-challenge/backend
   npm install
   ```
   ```sh
   cd tarent-challenge/backend
   npm install
   ```
4. Build the backend
   ```sh
   npm run build
   ```
5. **Important**! Copy `.env.example` to `.env` in **both** folders */frontend* and */backend*
   ```sh
   cp .env.example .env
   ```
   ```powershell
   Copy-Item ".env.example" -NewName ".env"
   ```
6. Start the backend
   ```sh
   npm start
   ```
5. Start the frontend
   ```sh
   npm start
   ```

### Credentials
There are two users. **admin** and **user**. Both use the password **password**
### Tests

All API operations are covered with basic unit tests using jest. In order to run them run
```sh
npm run test
```

### Pulling the repo

In order to fast-forward this repo and its submodules run 
```sh
git pull
git submodule update --remote --merge
```

### Generating API docs

You can regenerate the API documentation in case of changes to the swagger yaml.
```sh
npm run gen-docs
```

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## API Documentation
The generated REST API documentation is generated can be found [here][api-docs]
## Security Concerns

A few security concerns come to my mind.  

* CORS  
Origin should be limited to the domain the client is running on. In this case `http://localhost:3000`
* CSRF  
A random token should be double posted through cookies and http headers to prevent CSRF attacks.
* Check request bodies  
To prevent crashes XSS or DOS attacks, all request bodies should be tested against plausibility and rejected if they contain invalid or malformed data.
* HTTPS  
In a production environment a secured connection should be used.
* Authentication  
The API should be only accessible by authenticated users.
* Authorization  
The API should be authorized based on permissions to prevent leakage of sensitive information.
* Software Integrity  
The code should be unit tested to ensure a degree of integitry in order to prevent bugs slipping into production that could be exploited.
* Access Loggin  
To recognize DOS attempts or other malicious access, sufficient logging should be deployed on the serverside.
* Injection  
Forms should be sanitized to prevent injection. (react does sanitize form inputs).


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [X] UI
- [X] REST API
    - [X] Unit tests
- [X] Documentation
    - [X] Swagger API docs.
    - [X] Security concerns.

See the [open issues](https://github.com/C5H8NNaO4/tarent-challenge/issues) for a full list of proposed features (and known issues).

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



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Moritz Roessler - [@statelesscloud](https://twitter.com/statelesscloud) - moritz.roessler@gmail.com

Project Link: [https://github.com/C5H8NNaO4/tarent-challenge](https://github.com/C5H8NNaO4/tarent-challenge)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* []()
* []()
* []()

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/C5H8NNaO4/tarent-challenge.svg?style=for-the-badge
[contributors-url]: https://github.com/C5H8NNaO4/tarent-challenge/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/C5H8NNaO4/tarent-challenge.svg?style=for-the-badge
[forks-url]: https://github.com/C5H8NNaO4/tarent-challenge/network/members
[stars-shield]: https://img.shields.io/github/stars/C5H8NNaO4/tarent-challenge.svg?style=for-the-badge
[stars-url]: https://github.com/C5H8NNaO4/tarent-challenge/stargazers
[issues-shield]: https://img.shields.io/github/issues/C5H8NNaO4/tarent-challenge.svg?style=for-the-badge
[issues-url]: https://github.com/C5H8NNaO4/tarent-challenge/issues
[license-shield]: https://img.shields.io/github/license/C5H8NNaO4/tarent-challenge.svg?style=for-the-badge
[license-url]: https://github.com/C5H8NNaO4/tarent-challenge/blob/master/LICENSE.txt
[linkedin-url]: https://linkedin.com/in/moritz-roessler-666b18175
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555

[api-docs]: https://c5h8nnao4.github.io/tarent-challenge/docs/index.html
[product-screenshot]: images/screenshot.jpg