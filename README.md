import os

# Directory structure
project_dir = "/mnt/data/virtual_vocation_venture"
os.makedirs(project_dir, exist_ok=True)

# HTML content
html_content = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Virtual Vocation Venture</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="slide" id="slide1">
        <div class="title">Virtual Vocation Venture</div>
        <div class="mission-statement">Our mission statement<br>some things</div>
        <div class="image">
            <img src="path/to/image1.jpg" alt="People working together">
        </div>
        <div class="tagline">Onward to your Destiny</div>
    </div>
    <div class="slide" id="slide2">
        <div class="title">Pick your Path</div>
        <div class="options">
            <div class="hexagon">Military</div>
            <div class="hexagon">College Graduates</div>
            <div class="hexagon">Española</div>
            <div class="hexagon">Rezi</div>
            <div class="hexagon">Search Jobs</div>
        </div>
    </div>
    <div class="slide" id="slide3">
        <div class="title">About Us</div>
        <div class="description">
            At Contoso, we empower organizations to foster collaborative thinking to further drive workplace innovation. By closing the loop and leveraging agile frameworks, we help business grow organically and foster a consumer-first mindset.
        </div>
        <div class="image">
            <img src="path/to/image2.jpg" alt="People working in an open office">
        </div>
    </div>
    <div class="slide" id="slide4">
        <div class="title">Services</div>
        <div class="services">
            <div class="hexagon">O*Net</div>
            <div class="hexagon">Core Signal</div>
            <div class="hexagon">Rezi</div>
            <div class="hexagon">Job Board Plugin</div>
            <div class="hexagon">Job Tracker</div>
        </div>
    </div>
    <div class="slide" id="slide5">
        <div class="title">Contact Us</div>
        <div class="section">
            <div class="icon">Calculator</div>
            <div class="text">Envision multimedia-based expertise and cross-media growth strategies<br>Visualize quality intellectual capital<br>Engage worldwide methodologies with web-enabled technologies</div>
        </div>
        <div class="section">
            <div class="icon">Graph</div>
            <div class="text">Pursue scalable customer service through sustainable strategies<br>Engage top-line web services with cutting-edge deliverables</div>
        </div>
        <div class="section">
            <div class="icon">Chain</div>
            <div class="text">Cultivate one-to-one customer service with robust ideas<br>Maximize timely deliverables for real-time schemas</div>
        </div>
    </div>
    <div class="slide" id="slide6">
        <div class="title">Mission</div>
        <div class="description">
            <div class="column">Develop winning strategies to keep ahead of the competition<br>Capitalize on low-hanging fruit to identify a ballpark value<br>Visualize customer directed convergence</div>
            <div class="column">Iterative approaches to corporate strategy<br>Establish a management framework from the inside</div>
        </div>
    </div>
    <div class="slide" id="slide7">
        <div class="title">O*net</div>
        <div class="design-element">Hexagon</div>
    </div>
    <div class="slide" id="slide8">
        <div class="title">Rezi</div>
        <div class="screenshot">
            <img src="path/to/image3.jpg" alt="Resume building interface">
        </div>
        <div class="menu">
            <div class="menu-item">Create new resume</div>
            <div class="menu-item">My dashboard</div>
            <div class="menu-item">Sample library</div>
            <div class="menu-item">Review my resume</div>
            <div class="menu-item">AI interview</div>
            <div class="menu-item">Refer and earn</div>
        </div>
    </div>
    <div class="slide" id="slide9">
        <div class="title">Summary</div>
        <div class="description">
            At Contoso, we believe in giving 110%. By using our next-generation data architecture, we help organizations virtually manage agile workflows. We thrive because of our market knowledge and great team behind our product. As our CEO says, 'Efficiencies will come from proactively transforming how we do business.'
        </div>
        <div class="image">
            <img src="path/to/image4.jpg" alt="People working in an office">
        </div>
    </div>
    <div class="slide" id="slide10">
        <div class="title">Thank you</div>
        <div class="contact-information">
            Mirjam Nilsson<br>mirjam@contoso.com<br>www.contoso.com
        </div>
    </div>
</body>
</html>
"""

# CSS content
css_content = """
body {
    font-family: Arial, sans-serif;
}

.slide {
    margin: 50px;
    border: 1px solid #ccc;
    padding: 20px;
    border-radius: 10px;
}

.title {
    font-weight: bold;
    font-size: 2em;
    color: darkblue;
}

.mission-statement, .description, .contact-information {
    font-size: 1.2em;
    color: darkblue;
}

.image img {
    max-width: 100%;
    border-radius: 10px;
}

.tagline {
    font-size: 1em;
    color: darkblue;
    border: 2px solid darkblue;
    padding: 10px;
    border-radius: 10px;
}

.hexagon {
    display: inline-block;
    width: 100px;
    height: 100px;
    background: orange;
    margin: 10px;
    text-align: center;
    line-height: 100px;
    color: white;
    clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
}

.options .hexagon {
    background: lightgrey;
    color: darkblue;
}

.section {
    margin: 20px 0;
}

.icon {
    font-size: 1.5em;
    margin-right: 10px;
}

.column {
    display: inline-block;
    width: 45%;
    vertical-align: top;
}

.menu-item {
    margin: 10px 0;
    font-size: 1.1em;
    color: darkblue;
}
"""

# Write HTML and CSS files
with open(os.path.join(project_dir, "index.html"), "w") as file:
    file.write(html_content)

with open(os.path.join(project_dir, "style.css"), "w") as file:
    file.write(css_content)

print(f"Project created at {project_dir}")
