<div class="homePage">
    <div class="section01">
        <div class="leftContent">
            <div class="about-home">
                <div>
                    <b>Kola</b> is a comprehensive integration solution that simplifies your digital transformation journey. The Kola extension for Visual Studio Code (Kola for VS Code) enables developers to utilize the popular Visual Studio Code editor for integration development, enhancing the overall experience. This AI-assisted development environment offers a faster, customizable, and more intuitive experience, boosting productivity in integration development.
                    Kola provides a range of features that streamline coding tasks, enhance code quality, and reduce time spent on error-prone processes. By leveraging AI capabilities, Kola empowers developers to focus on high-value tasks, accelerating digital transformation efforts.
                    <div class="linkSet2" onclick="location.href='{{base_path}}/get-started/quick-start-guide';">
                        <a href="get-started/quick-start-guide"><h3>Quick Start Guide ></h3></a>
                        <p>
                            Get started with Kola by running a simple integration use case in your local environment.
                        </p>
                    </div>
                </div>
                <div  style="text-align:right">
                    <a href="{{base_path}}/assets/img/introduction/kola.png"><img src="{{base_path}}/assets/img/introduction/kola.png" alt="Kola" width="95%"></a>
                </div>
            </div>
        </div>
    </div>
    <hr class="rounded">
    <div class="section02">
        <div class="rightContent">
                <div class="about-home">
                    <div  style="text-align:left">
                        <a href="{{base_path}}/assets/img/introduction/low-code.gif"><img src="{{base_path}}/assets/img/introduction/low-code.gif" alt="low-code" width="90%" style="padding-top: 60px" ></a>
                    </div>
                    <div>
                        <h3>Low-code integration development</h3>
                        <p>
                            Kola offers a user-friendly, streamlined environment for building integrations with minimal coding, accessible to both experienced developers and beginners. Here’s how Kola’s low-code features simplify integration development:
                        </p>
                        <ul>
                            <li><b>Design Visually:</b> Kola’s interface lets users design integrations visually, simplifying flow creation and management.</li>
                            <li><b>Pre-built Connectors:</b> Kola offers connectors for easy integration with various systems and services.</li>
                            <li><b>Reuse Components:</b> Create and share reusable components across integrations, saving time and effort.</li>
                            <li><b>Automate Testing:</b> Automated testing helps identify and fix issues early.</li>
                            <li><b>AI-Assisted Development:</b> Kola’s AI provides smart suggestions to boost coding efficiency and accuracy.</li>
                        </ul>
                    </div>
                </div>
        </div>
    </div>
     <hr class="rounded">
     <div class="section02">
        <div class="leftContent">
                <div class="about-home">
                    <div>
                        <h3>AI-assisted development</h3>
                        <p>
                            Kola leverages AI to streamline coding tasks, improve code quality, and reduce time on error-prone processes. Here’s how Kola’s AI capabilities make a difference:
                        </p>
                        <ul>
                            <li><b>Code Suggestions and Autocompletion:</b> Kola’s AI provides context-aware suggestions, helping developers code faster with real-time prompts for methods, properties, and configurations.</li>
                            <li><b>Error Detection and Fix Recommendations:</b> AI identifies errors and suggests fixes early, enhancing code quality and minimizing debugging needs.</li>
                            <li><b>Pattern Recognition and Code Optimization:</b> Kola’s AI detects code patterns and suggests optimizations, boosting performance and aiding code standardization.</li>
                            <li><b>Natural Language Code Search and Commands:</b> Developers can search for code snippets or methods using natural language, reducing documentation time and accelerating onboarding.</li>
                            <li><b>Smart Refactoring and Code Restructuring:</b> Kola’s AI suggests refactoring options, enabling a cleaner, more maintainable codebase.</li>
                        </ul>
                    </div>
                    <div  style="text-align:right">
                        <a href="{{base_path}}/assets/img/introduction/ai.gif"><img src="{{base_path}}/assets/img/introduction/ai.gif" alt="AI" width="90%" style="padding-top: 60px; padding-right: 50px" ></a>
                    </div>
                </div>
        </div>
    </div>
    <hr class="rounded">
    <div class="section02">
        <div class="rightContent">
                <div class="about-home">
                    <div  style="text-align:left">
                        <a href="{{base_path}}/assets/img/introduction/ballerina.png"><img src="{{base_path}}/assets/img/introduction/ballerina.png" alt="ballerina" width="50%" style="padding-top: 250px" ></a>
                    </div>
                    <div>
                        <h3>Leverage the Power of Ballerina</h3>
                        <p>
                            Kola uses <a href="https://ballerina.io">Ballerina</a>, a language designed for seamless integration development, making API-driven, cloud-native workflows simpler and more efficient. Ballerina offers:
                        </p>
                        <ul>
                            <li><b>Integration-Centric Syntax:</b> Optimized syntax with constructs like workers, channels, and error handling for clear API orchestration.</li>
                            <li><b>Cloud-Native Design:</b> Supports HTTP, WebSocket, gRPC, and Kafka for API-first, microservices-ready development.</li>
                            <li><b>Visual Flow Representation:</b> Graphical views that show data flow and logic for complex workflows.</li>
                            <li><b>Observability and Resilience:</b> Built-in tracing, metrics, and logging for efficient monitoring.</li>
                            <li><b>Unified Data Handling:</b> Simplifies data transformations for diverse integrations.</li>
                            <li><b>Testing and Deployment Tools:</b> Integrated tools for scalable, reliable cloud deployment.</li>
                        </ul>
                    </div>
                </div>
        </div>
    </div>
</div>
{% raw %}
<style>
.md-sidebar.md-sidebar--primary {
    display: none;
}
.md-sidebar.md-sidebar--secondary{
    display: none;
}
.section02 {
    display: flex;
    justify-content: space-between;
}
header.md-header .md-header__button:not([hidden]) {
    /* display: none; */
}
.about-home {
    display: flex;
}
.about-home div:first-child {
    width: 50%;
    padding-top: 20px;
}
.about-home div:nth-child(2) {
    width: 50%;
}
@media screen and (max-width: 76.1875em) {
    .md-sidebar.md-sidebar--primary {
        display: block;
    }
}
@media screen and (max-width: 945px) {
    .about-home div:first-child {
        width: 100%;
    }
    .about-home div:nth-child(2) {
        width: 100%;
    }
    .about-home {
        flex-direction: column;
    }
    .md-typeset a {
        background-position-x: left;
    }
    .download-btn-wrapper {
        display: block;
        text-align: center;
    }
}
.md-typeset h1{
    visibility: hidden;
    margin-bottom: 0;
}
.md-search-result__article.md-typeset h1{
    visibility: visible;
}
</style>
{% endraw %}