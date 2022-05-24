<div id="top"></div>

[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://vebko.org/en/Default.aspx">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Vebko Screen Sharing Service</h3>


  <p align="center">
    A screen sharing service for Vebko company using WebRTC.
    <br />
    <a href="https://vebko.org:8088/presenter.html">View Demo as a presenter</a>
    <a href="https://vebko.org:8088/viewer.html">View Demo as a viewer</a>
  </p>
</div>

https://user-images.githubusercontent.com/14248281/170082470-c46a59c4-1c8d-4924-818d-b19b419fd127.mp4


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
      </ul>
      <ul>
        <li><a href="#Expose-WebRTC-Screen-Sharing-on-HTTPS">Expose WebRTC Screen Sharing on HTTPS</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://vebko.org/en/Software.aspx)

Web-based screen sharing service for Vebko
This project uses WebRTC for share screen and sounds.

Here's why:
* WebRTC has less delay than other alternatives.
* Works on all devices and browsers without any requirments :smile:

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

For running this service you have to install the requirments.


### Installation

to install front and back:

1. Clone the repe
2. Install NPM packages
 
   ```sh
   npm install
   ```
3. Serv the files (you can use http-server and include .certs)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- Expose WebRTC Screen Sharing on HTTPS -->

### Expose WebRTC Screen Sharing on HTTPS

1. Generate a `self-signed certificate`

```bash
# install openssl 4 ubuntu
apt install openssl
# install openssl 4 mac
brew install openssl

# self-signed certificate
openssl genrsa -out key.pem
openssl req -new -key key.pem -out csr.pem
openssl x509 -req -days 9999 -in csr.pem -signkey key.pem -out cert.pem
rm csr.pem

# https://www.sslchecker.com/certdecoder
```

2. run `server.js` on `https`

3. Change Certs inside cert directory


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


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/taherfattahi/WebRTC-Screen-Sharing/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/nimk
[product-screenshot]: images/screenshot.png
