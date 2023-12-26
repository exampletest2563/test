# Module 1. 📜 History Of The Web

## Internet & World Wide Web

The evolution of the `World Wide Web` (`Web`) has been a remarkable journey, shaping the way information is shared, accessed, and experienced globally.

In 1989, `Tim Berners-Lee`, a British computer scientist, proposed the concept of a `decentralized information system` that would eventually become the `World Wide Web`. His vision included the use of `hypertext` to link documents and a system of `uniform resource identifiers` to uniquely identify resources.

In 1990, `Tim Berners-Lee` implemented the first successful communication between a `Hypertext Transfer Protocol` (`HTTP`) client and server, effectively creating the foundation for the `Web`. The first website, `info.cern.ch`, and the first web browser, `WorldWideWeb` (later renamed `Nexus`), were developed in 1991.

There is a difference between `Internet` and `Web` as `Internet` refers to a network of networks that connects devices all over the world, while `Web` is an information system that enables information sharing over the `Internet`.

## Web Page, Web Site & Web Application

## HTML, CSS & JS

`HTML` (HyperText Markup Language) is used to define `the content` of Web pages. It uses elements, tags and attributes to define building blocks/components such as `headings`, `paragraphs`, `images`, `links`, and more.

`HTML Example`

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Document</title>
		<meta charset="UTF-8">
	</head>
	<body>
		<h1>HTML Introduction</h1>
	    <p>This is a basic HTML document.</p>
	</body>
</html>
```

`CSS` (Cascading Style Sheets) is used to specify `the layout` of Web pages. `CSS` is responsible for styling HTML elements, controlling `layout`, `design`, and `presentation`. `CSS` was introduced to separate the presentation of Web documents from their structure.

`CSS Example`

```css
body {
	font-family: 'Arial';
	background-color: white;
}

h1 {
	color: black;
	text-align: center;
}

p {
	font-size: 14px;
}
```

`JS` (JavaScript) is used to program `the behavior` of Web pages (client-side interactivity), significantly enhancing the user experience.

`JavaScript Example`

```js
document.getElementById("demo").style.visibility = "hidden";
```

`Separation of Concerns` is a design principle for separating a computer program into distinct sections. Each section addresses a separate concern, a set of information that affects the code of a computer program.

`HTML` is mainly used for organization of webpage content, `CSS` is used for definition of content presentation style, and `JS` defines how the content interacts and behaves with the user. Historically, this was not the case: prior to the introduction of `CSS`, `HTML` performed both duties of defining semantics and style.

File Naming Conventions:
- `HTML` - `index.html`;
- `CSS` - `styles.css`;
- `JS` - `app.js`, `main.js` or `script.js`.

## Front-End & Back-End

`Front-end development`, or `client-side development`, focuses on the `user interface and user experience` of a website. It involves crafting the `visual elements`, `layouts`, and `interactivity` that users directly interact with.

Technologies & Languages:
- `HTML5`;
- `CSS3`;
- `JavaScript`.

Front-end developers often utilize frameworks and libraries like `React`, `Angular`, or `Vue.js` to streamline development, manage state, and create modular and reusable components.

`Back-end development`, or `server-side development`, focuses on `server operations`, `databases`, and `application logic`. It ensures `data processing, storage, and retrieval`, as well as `handling business logic` that powers the application.

Technologies & Languages:
- `Node.JS`;
- `Python`;
- `PHP`;
- `Java`;
- `C#`;

Front-end and back-end communicate via the `Hypertext Transfer Protocol` (HTTP). The front-end sends requests, and the back-end responds with data or performs actions.

Full-stack development includes front-end and back-end development.

## Client-Server Architecture

## User-Agent String

The `User-Agent string` is an `HTTP header field` that browsers send to servers to identify themselves. It includes details about the browser, operating system, and sometimes additional information about the device.

A typical User-Agent string consists of the following components:
- `Browser Information`: Specifies the name and version of the browser.
- `Operating System`: Indicates the operating system running on the client device.
- `Device Information`: In some cases, details about the device, such as model or form factor.

`Example`

```
Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36
```

In this example:
- `Mozilla/5.0`: Represents compatibility.
- `(Windows NT 10.0; Win64; x64)`: Indicates the Windows 10 operating system and 64-bit architecture.
- `AppleWebKit/537.36 (KHTML, like Gecko)`: Denotes the browser engine.
- `Chrome/91.0.4472.124`: Specifies the Chrome browser version.
- `Safari/537.36`: Highlights compatibility with the Safari browser.

## Browser Wars

The late '90s and early 2000s saw intense competition among web browsers, known as the "Browser Wars". Internet Explorer, Netscape Navigator, and later Firefox, Chrome, Safari, and Opera battled for dominance, driving innovation and pushing the boundaries of web technologies.

## The Future Of Web

As the Web expanded, ensuring compatibility across different browsers became a priority. The establishment of web standards by organizations like the World Wide Web Consortium (W3C) aimed to create consistency in how browsers interpreted and displayed web content.

The World Wide Web Consortium (W3C) plays a pivotal role in developing and maintaining web standards that ensure interoperability and accessibility across different browsers and devices.

- AI
- Mobile Usage

The advent of smartphones and tablets brought about a shift in user behavior, emphasizing the need for mobile-friendly websites. Responsive web design emerged as a best practice, enabling websites to adapt seamlessly to various screen sizes and orientations.