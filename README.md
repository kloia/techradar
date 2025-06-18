# Kloia Technology Radar

[![AGPL License](https://badgen.net/github/license/thoughtworks/build-your-own-radar)](https://github.com/thoughtworks/build-your-own-radar)

An interactive technology radar showcasing [Kloia's](https://kloia.com) expertise and recommendations in DevOps, Cloud Native, and Platform Engineering practices.

This application is built upon the [Build Your Own Radar](https://github.com/thoughtworks/build-your-own-radar) library by ThoughtWorks, adapted to display Kloia's technology recommendations and insights.

## About Kloia Technology Radar

The Kloia Technology Radar is a visual representation of our technology landscape, showcasing the tools, techniques, platforms, and frameworks that we recommend for modern software development and infrastructure practices. 

Our radar is organized into four quadrants:
- **Techniques**: Development practices, methodologies, and approaches
- **Tools**: Software development and operations tools
- **Platforms**: Infrastructure and runtime platforms
- **Languages & Frameworks**: Programming languages and development frameworks

Each technology is positioned in one of four rings based on our recommendation:
- **Adopt**: Technologies we have high confidence in and actively use
- **Trial**: Technologies worth pursuing and experimenting with
- **Assess**: Technologies to explore and understand their potential
- **Hold**: Technologies to approach with caution or avoid

## Live Demo

Visit [Kloia Technology Radar](https://your-radar-url.com) to explore our current technology recommendations.

## About the Data

Our radar data includes:
- **Technology Name**: The name of the tool, technique, platform, or framework
- **Ring**: Our recommendation level (Adopt, Trial, Assess, Hold)  
- **Quadrant**: The category it belongs to
- **Status**: Whether it's new to our radar or has moved position
- **Description**: Our assessment and reasoning for the placement

## Development

### Prerequisites

- Node.js (see `.nvmrc` for the specific version)
- npm

### Running Locally

```bash
# Clone the repository
git clone [your-repository-url]
cd kloia-technology-radar

# Install dependencies
npm install

# Run in development mode
npm run dev
```

The application will be available at `http://localhost:8080`.

### Available Scripts

All tasks are defined in `package.json`:

- `npm run dev` - Run application in development mode with hot reloading
- `npm run build` - Build the application for production
- `npm run quality` - Run linter and unit tests
- `npm test` - Run unit tests
- `npm run test:ci` - Run tests in CI mode

### Code Quality

- `npm run lint` - Run ESLint
- `npm run format` - Format code with Prettier
- `npm run quality` - Run both linting and tests

## Docker

### Building and Running with Docker

```bash
# Build the Docker image
docker build -t kloia-technology-radar .

# Run the container
docker run -p 8080:80 kloia-technology-radar

# Access the application
open http://localhost:8080
```

### Using Docker Compose

```bash
# Start the application
docker-compose up

# Access the application
open http://localhost:8080
```

## Deployment

The application can be deployed to any static hosting service or container platform:

- **Static Hosting**: Netlify, Vercel, GitHub Pages
- **Container Platforms**: AWS ECS, Google Cloud Run, Azure Container Instances
- **Kubernetes**: Use the provided Kubernetes manifests

### Environment Variables

Optional environment variables for advanced configuration:

```bash
# Google Analytics (optional)
export GTM_ID=[Google Tag Manager ID]

# Adobe Launch (optional)  
export ADOBE_LAUNCH_SCRIPT_URL=[Adobe Launch URL]

# Custom rings (optional)
export RINGS='["Adopt", "Trial", "Assess", "Hold"]'

# Custom quadrants (optional)
export QUADRANTS='["Techniques", "Platforms", "Tools", "Languages & Frameworks"]'
```

## Technology Stack

- **Frontend**: HTML5, CSS3 (SCSS), JavaScript (ES6+)
- **Build Tool**: Webpack
- **Visualization**: D3.js
- **Styling**: Sass, CSS Grid, Flexbox
- **Font**: Inter (for modern, clean typography)

## Architecture

The application follows a modular architecture:

```
src/
├── models/          # Data models (Radar, Quadrant, Ring, Blip)
├── graphing/        # Visualization and rendering logic
├── util/            # Utility functions and helpers
├── stylesheets/     # SCSS styles and theming
├── images/          # Static assets and logos
└── exceptions/      # Error handling
```

## Contributing

We welcome contributions to improve the radar:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Run tests (`npm run quality`)
5. Commit your changes (`git commit -m 'Add amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

### Development Guidelines

- Follow the existing code style
- Write tests for new functionality
- Update documentation as needed
- Ensure all quality checks pass

## License

This project is licensed under the AGPL License - see the [LICENSE.md](LICENSE.md) file for details.

## Attribution

This application is built upon the [Build Your Own Radar](https://github.com/thoughtworks/build-your-own-radar) project by [ThoughtWorks](https://www.thoughtworks.com/). We are grateful for their excellent open-source contribution to the technology community.

The original Build Your Own Radar project is also licensed under the AGPL License.

## About Kloia

[Kloia](https://kloia.com) is a technology consultancy specializing in DevOps, Cloud Native technologies, and Platform Engineering. We help organizations transform their software delivery practices and infrastructure to achieve faster, more reliable deployments.

### Our Services

- **DevOps Transformation**: Implementing modern DevOps practices and toolchains
- **Cloud Migration**: Moving applications and infrastructure to the cloud
- **Platform Engineering**: Building internal developer platforms
- **Observability**: Implementing monitoring, logging, and tracing solutions
- **Application Modernization**: Modernizing legacy applications for the cloud
- **Testing Solutions**: Automated testing strategies and implementation

### Connect with Us

- Website: [kloia.com](https://kloia.com)
- Blog: [kloia.com/blog](https://kloia.com/blog)
- LinkedIn: [linkedin.com/company/kloia](https://linkedin.com/company/kloia)
- Contact: [kloia.com/contact](https://kloia.com/contact)

---

*This radar represents our current thinking and is updated regularly to reflect our evolving technology landscape and recommendations.*
