<h1 align="center">
  <br>
  <a href="https://github.com/karthikuj/sasori"><img src="./resources/sasori-logo.png" alt="Sasori Logo" width="200" /></a>
  <br>
  Sasori: Dynamic Web Crawler
  <br>
</h1>

<p align="center"><img src="./resources/sasori.gif" alt="Sasori Demo" width="700" /></p>

## Project Description:
Sasori is a powerful and flexible dynamic web crawler built on Puppeteer. It allows you to automate the crawling of web applications, even those behind authentication, offers seamless integration with security testing tools like Zaproxy or Burp Suite and provides customizable configurations for enhanced flexibility.


## Features
- **Dynamic Crawling:** Sasori excels at crawling dynamic web applications, handling AJAX-loaded content, and interacting with complex user interfaces.

- **Authentication Support:** Easily spider applications behind authentication barriers by passing the puppeteer recording for the login sequence.

- **Proxy Integration:** Sasori provides the option to set up a proxy server, allowing you to route requests through tools like Zaproxy or Burp Suite for security testing.

- **State-Based Navigation:** The project is designed around a state-based system, keeping track of URLs, DOM structures, and interactable elements for efficient crawling.

- **Efficient Endpoint Coverage:** Utilizes efficient algorithms for intelligent crawling, ensuring coverage of more endpoints while maintaining speed.

- **Crawl Customization:** Allows you to customize what elements to interact with to target specific use cases.


## Getting Started:
To get started with Sasori, follow these steps:

### Recommended
1. Install the package globally:
```bash
npm install -g sasori-crawl
```

2. Create Sasori's configuration file:
```bash
sasori init
```

3. Edit the configuration file. Check [Configuration](#configuration)

4. Run Sasori:
```bash
sasori start --config /path/to/config.json
```

### Alternative
1. Clone the repository:
```bash
git clone https://github.com/karthikuj/sasori.git
```

2. Install dependencies:
```bash
cd sasori
npm install
```

3. Configure Sasori by editing the configuration file in the `config` directory. Check [Configuration](#configuration).

4. Run Sasori:
```bash
node . start --config ./config/config.json
```


## Configuration:
Sasori offers various configuration options to customize its behavior. These include:

- Headless and Headful modes.
- Proxy server settings for integration with Zaproxy or Burp Suite.
- Customize crawl elements.
- Authentication recording.
- Max duration.
- Regexes for scope management.


## Contributing:
Contributions to Sasori are welcome! If you encounter any bugs, have feature requests, or would like to contribute code improvements, please follow the guidelines in the [CONTRIBUTING.md](CONTRIBUTING.md) file.


## License:
This project is licensed under the [MIT License](LICENSE).