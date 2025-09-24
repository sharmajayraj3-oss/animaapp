# animaapp
# My code for RPA website 
import React from "react";

// Services offered
const services = [
  "RPA Consulting & Strategy",
  "Workflow Automation Design",
  "Bot Development & Deployment",
  "Multi-Tool RPA Integration (ServiceNow, UiPath, Power Automate)",
  "Support & Maintenance",
  "Training & Enablement",
];

// Case studies highlighting multi-tool use cases
const caseStudies = [
  {
    title: "Automating IT Service Management",
    summary:
      "Implemented multi-tool automation using ServiceNow RPA and UiPath bots for seamless ITSM workflows, improving SLA adherence by 45%.",
  },
  {
    title: "Finance Process Automation",
    summary:
      "Combined Power Automate and UiPath to streamline invoice processing and approvals, reducing manual effort by 60%.",
  },
  {
    title: "Customer Support Automation",
    summary:
      "Deployed ServiceNow RPA and Power Automate bots to accelerate case resolution, improving customer satisfaction scores significantly.",
  },
];

// Blog posts covering a broad range of RPA topics
const blogPosts = [
  {
    title: "Choosing the Right RPA Tool for Your Business",
    date: "Sep 2025",
  },
  {
    title: "Best Practices for Multi-Platform RPA Automation",
    date: "Aug 2025",
  },
  {
    title: "Getting Started with ServiceNow, UiPath, and Power Automate",
    date: "July 2025",
  },
];

// Logos for RPA tools used
const logos = [
  {
    alt: "ServiceNow RPA",
    src: "https://upload.wikimedia.org/wikipedia/commons/a/a5/Servicenow_logo.svg",
  },
  {
    alt: "UiPath",
    src: "https://upload.wikimedia.org/wikipedia/commons/5/52/UiPath_Logo.svg",
  },
  {
    alt: "Power Automate",
    src: "https://upload.wikimedia.org/wikipedia/commons/3/3a/Microsoft_Power_Automate_Logo.svg",
  },
];

// Technologies component showing all tool logos
function AutomationTechLogos() {
  return (
    <section
      id="automation-tech"
      style={{ maxWidth: "900px", margin: "40px auto", padding: "0 20px", textAlign: "center" }}
    >
      <h3 style={{ marginBottom: "20px" }}>Our Automation Technologies</h3>
      <p style={{ marginBottom: "30px" }}>
        NeuraBots Pvt. Ltd. empowers your business with leading RPA tools — ServiceNow RPA, UiPath, and Microsoft Power Automate — choosing the right tool for your unique automation needs.
      </p>
      <div style={{ display: "flex", justifyContent: "center", gap: "40px", flexWrap: "wrap" }}>
        {logos.map(({ alt, src }) => (
          <img
            key={alt}
            src={src}
            alt={alt}
            style={{ height: "60px", width: "auto", filter: "brightness(0) invert(0.2)" }}
          />
        ))}
      </div>
    </section>
  );
}

// Benefit item component
const Benefit = ({ icon, label }) => (
  <div style={{ maxWidth: "150px", textAlign: "center", marginBottom: "20px" }}>
    <div style={{ fontSize: "2.5rem" }}>{icon}</div>
    <p style={{ fontWeight: "600" }}>{label}</p>
  </div>
);

// Navigation link styles
const navLinkStyle = {
  color: "white",
  marginLeft: "20px",
  textDecoration: "none",
  fontWeight: "600",
  fontSize: "1rem",
};

// Buttons styling
const buttonPrimary = {
  display: "inline-block",
  backgroundColor: "#ff7f50",
  color: "white",
  padding: "14px 28px",
  marginRight: "15px",
  borderRadius: "6px",
  cursor: "pointer",
  textDecoration: "none",
  fontWeight: "600",
  fontSize: "1.1rem",
};

const buttonSecondary = {
  display: "inline-block",
  backgroundColor: "white",
  color: "#004080",
  padding: "14px 28px",
  borderRadius: "6px",
  cursor: "pointer",
  textDecoration: "none",
  fontWeight: "600",
  fontSize: "1.1rem",
  border: "2px solid #004080",
};

const inputStyle = {
  padding: "14px",
  borderRadius: "6px",
  border: "1px solid #ccc",
  fontSize: "1rem",
};

function App() {
  return (
    <div style={{ fontFamily: "Arial, sans-serif", lineHeight: "1.6", color: "#333" }}>
      {/* Header with logo */}
      <header
        style={{
          padding: "20px 40px",
          backgroundColor: "#003366",
          color: "#fff",
          display: "flex",
          justifyContent: "space-between",
          alignItems: "center",
          flexWrap: "wrap",
        }}
      >
        {/* Company Logo (ensure neurabots-logo.jpeg is in your public folder) */}
        <img
          src="/neurabots-logo.jpeg"
          alt="NeuraBots Logo"
          style={{
            height: "60px",
            marginRight: "20px",
            flex: "1 1 200px",
          }}
        />
        <nav style={{ flex: "2 1 400px", textAlign: "right" }}>
          <a href="#services" style={navLinkStyle}>
            Services
          </a>
          <a href="#technology" style={navLinkStyle}>
            Technology
          </a>
          <a href="#automation-tech" style={navLinkStyle}>
            Tools
          </a>
          <a href="#case-studies" style={navLinkStyle}>
            Case Studies
          </a>
          <a href="#best-practices" style={navLinkStyle}>
            Best Practices
          </a>
          <a href="#blog" style={navLinkStyle}>
            Blog
          </a>
          <a href="#about" style={navLinkStyle}>
            About Us
          </a>
          <a href="#contact" style={navLinkStyle}>
            Contact
          </a>
        </nav>
      </header>

      {/* Hero Section */}
      <section
        style={{
          backgroundColor: "#004080",
          color: "white",
          padding: "80px 40px",
          textAlign: "center",
        }}
      >
        <h2 style={{ fontSize: "2.5rem", marginBottom: "16px" }}>
          Unlock Business Efficiency with Multi-Platform RPA Automation
        </h2>
        <p style={{ fontSize: "1.25rem", marginBottom: "32px" }}>
          Harness the power of ServiceNow RPA, UiPath, and Power Automate to streamline workflows, reduce errors, and drive digital transformation.
        </p>
        <div>
          <a href="#contact" style={buttonPrimary}>
            Free Consultation
          </a>
          <a href="#services" style={buttonSecondary}>
            Our Services
          </a>
        </div>
      </section>

      {/* Value Proposition */}
      <section
        style={{
          maxWidth: "900px",
          margin: "40px auto",
          padding: "0 20px",
          textAlign: "center",
        }}
      >
        <p style={{ fontSize: "1.1rem" }}>
          At NeuraBots Pvt. Ltd., we deliver tailored RPA solutions leveraging multiple best-in-class platforms to automate your unique business processes, ensuring scalability, reliability, and measurable value.
        </p>
        <div style={{ display: "flex", justifyContent: "space-around", marginTop: "30px", flexWrap: "wrap" }}>
          <Benefit icon="⚡" label="Improved Efficiency" />
          <Benefit icon="💰" label="Cost Savings" />
          <Benefit icon="🔄" label="Cross-Platform Flexibility" />
          <Benefit icon="🔐" label="Secure Automation" />
        </div>
      </section>

      {/* Services Overview */}
      <section id="services" style={{ backgroundColor: "#f0f4f8", padding: "40px 20px" }}>
        <h3 style={{ textAlign: "center", marginBottom: "30px" }}>Our Services</h3>
        <div
          style={{
            maxWidth: "900px",
            margin: "0 auto",
            display: "grid",
            gap: "20px",
            gridTemplateColumns: "repeat(auto-fit,minmax(280px,1fr))",
          }}
        >
          {services.map((service, idx) => (
            <div
              key={idx}
              style={{
                background: "white",
                padding: "20px",
                boxShadow: "0 2px 8px rgba(0,0,0,0.12)",
                borderRadius: "6px",
                textAlign: "center",
                fontWeight: "600",
              }}
            >
              {service}
            </div>
          ))}
        </div>
      </section>

      {/* Technology Spotlight */}
      <section id="technology" style={{ maxWidth: "900px", margin: "40px auto", padding: "0 20px" }}>
        <h3 style={{ marginBottom: "20px", textAlign: "center" }}>Our Approach to Technology</h3>
        <p style={{ textAlign: "center", marginBottom: "40px" }}>
          We expertly integrate multiple RPA platforms to choose the best fit for each business process, delivering seamless automation solutions that maximize ROI.
        </p>
        <div
          style={{
            textAlign: "center",
            backgroundColor: "#dbe9f4",
            padding: "30px",
            borderRadius: "8px",
            fontStyle: "italic",
            color: "#333",
          }}
        >
          [Your customized automation workflow diagrams or images can be placed here]
        </div>
      </section>

      {/* Automation Technologies Logos */}
      <AutomationTechLogos />

      {/* Case Studies Preview */}
      <section id="case-studies" style={{ backgroundColor: "#f0f4f8", padding: "40px 20px" }}>
        <h3 style={{ textAlign: "center", marginBottom: "30px" }}>Case Studies</h3>
        <div
          style={{
            maxWidth: "900px",
            margin: "0 auto",
            display: "grid",
            gap: "20px",
            gridTemplateColumns: "repeat(auto-fit,minmax(300px,1fr))",
          }}
        >
          {caseStudies.map((caseStudy, idx) => (
            <div
              key={idx}
              style={{
                background: "white",
                padding: "20px",
                boxShadow: "0 2px 8px rgba(0,0,0,0.12)",
                borderRadius: "6px",
              }}
            >
              <h4>{caseStudy.title}</h4>
              <p>{caseStudy.summary}</p>
              <a href="#contact" style={{ color: "#004080", fontWeight: "600" }}>
                Read More
              </a>
            </div>
          ))}
        </div>
      </section>

      {/* Best Practices Brief */}
      <section id="best-practices" style={{ maxWidth: "900px", margin: "40px auto", padding: "0 20px" }}>
        <h3 style={{ textAlign: "center", marginBottom: "20px" }}>Best Practices</h3>
        <p style={{ textAlign: "center" }}>
          We adhere to industry best practices such as modular workflow design, robust error handling, secure credential management, and scalable automation architectures across multiple RPA platforms.
        </p>
      </section>

      {/* Blog/Resources Preview */}
      <section id="blog" style={{ backgroundColor: "#f0f4f8", padding: "40px 20px" }}>
        <h3 style={{ textAlign: "center", marginBottom: "30px" }}>Latest Articles</h3>
        <div
          style={{
            maxWidth: "900px",
            margin: "0 auto",
            display: "grid",
            gap: "20px",
            gridTemplateColumns: "repeat(auto-fit,minmax(300px,1fr))",
          }}
        >
          {blogPosts.map((post, idx) => (
            <div
              key={idx}
              style={{
                background: "white",
                padding: "20px",
                boxShadow: "0 2px 8px rgba(0,0,0,0.12)",
                borderRadius: "6px",
              }}
            >
              <h4>{post.title}</h4>
              <p style={{ fontSize: "0.9rem", color: "#555" }}>{post.date}</p>
              <a href="#blog" style={{ color: "#004080", fontWeight: "600" }}>
                Read More
              </a>
            </div>
          ))}
        </div>
      </section>

      {/* About Us */}
      <section id="about" style={{ maxWidth: "900px", margin: "40px auto", padding: "0 20px" }}>
        <h3 style={{ textAlign: "center", marginBottom: "20px" }}>About NeuraBots Pvt. Ltd.</h3>
        <p style={{ textAlign: "center", maxWidth: "700px", margin: "0 auto" }}>
          NeuraBots Pvt. Ltd. is a leading automation consultancy delivering expert multi-platform RPA implementations using ServiceNow RPA, UiPath, and Power Automate. We empower businesses to automate smartly, scale quickly, and innovate continuously.
        </p>
      </section>

      {/* Contact Section */}
      <section
        id="contact"
        style={{
          backgroundColor: "#004080",
          color: "white",
          padding: "40px 20px",
          textAlign: "center",
        }}
      >
        <h3>Contact Us</h3>
        <form
          style={{
            maxWidth: "400px",
            margin: "20px auto",
            display: "flex",
            flexDirection: "column",
            gap: "10px",
          }}
          onSubmit={(e) => {
            e.preventDefault();
            alert("Thank you for contacting NeuraBots Pvt. Ltd.!");
          }}
        >
          <input type="text" placeholder="Name" required style={inputStyle} />
          <input type="email" placeholder="Email" required style={inputStyle} />
          <textarea placeholder="Your message" rows="4" required style={inputStyle} />
          <button type="submit" style={buttonPrimary}>
            Send Message
          </button>
        </form>
        <p>Phone: +1 (555) 123-4567 | Email: info@neurabots.com</p>
      </section>

      {/* Footer */}
      <footer
        style={{
          backgroundColor: "#003366",
          color: "white",
          textAlign: "center",
          padding: "20px 10px",
          marginTop: "40px",
        }}
      >
        <p>
          © {new Date().getFullYear()} NeuraBots Pvt. Ltd. All rights reserved. | Privacy Policy | Terms of Use
        </p>
      </footer>
    </div>
  );
}

export default App;

