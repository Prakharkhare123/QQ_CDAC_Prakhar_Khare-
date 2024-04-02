# QQ_CDAC_Prakhar_Khare-

import React from 'react';
import './App.css'; 
import 'bootstrap/dist/css/bootstrap.min.css'; 
import { FontAwesomeIcon } from '@fortawesome/react-fontawesome'; 
function App() {
  return (
    <div id="outer">
      <header className="header order-last" id="tm-header">
        <nav className="navbar">
          <div className="collapse navbar-collapse single-page-nav">
            <ul className="navbar-nav">
              <li className="nav-item">
                <a className="nav-link" href="#section-1">
                  <span className="icn">
                    <FontAwesomeIcon icon={['fas', 'air-freshener']} size="2x" />
                  </span>
                  Our Company
                </a>
              </li>
              <li className="nav-item">
                <a className="nav-link" href="#section-2">
                  <span className="icn">
                    <FontAwesomeIcon icon={['fab', 'battle-net']} size="2x" />
                  </span>
                  Our Work
                </a>
              </li>
              <li className="nav-item">
                <a className="nav-link" href="#section-3">
                  <span className="icn">
                    <FontAwesomeIcon icon={['far', 'images']} size="2x" />
                  </span>
                  Gallery
                </a>
              </li>
              <li className="nav-item">
                <a className="nav-link" href="#section-4">
                  <span className="icn">
                    <FontAwesomeIcon icon={['far', 'comments']} size="2x" />
                  </span>
                  Contact
                </a>
              </li>
            </ul>
          </div>
        </nav>
      </header>

      <button className="navbar-button collapsed" type="button">
        <span className="menu_icon">
          <span className="icon-bar"></span>
          <span className="icon-bar"></span>
          <span className="icon-bar"></span>
        </span>
      </button>

      <main id="content-box" className="order-first">
        {/* Add your other components here */}
      </main>
    </div>
  );
}

export default App;

---------------------------------------------------------------------------------------------------
//Banner Section

import React from 'react';

function BannerSection() {
  return (
    <div className="banner-section section parallax-window"
         data-parallax="scroll"
         data-image-src="img/section-1-bg.jpg"
         id="section-1">
      <div className="container">
        <div className="item">
          <div className="bg-blue-transparent logo-fa">
            <span><i className="fas fa-2x fa-atom"></i></span> Simply Amazed
          </div>
          <div className="bg-blue-transparent simple">
            <p>Your simplest HTML template, the most amazing page ever, yet free!</p>
          </div>
        </div>
      </div>
    </div>
  );
}

export default BannerSection;

-----------------------------------------------------------------------------------------------------------------------------------------------
 // App
 
import React from 'react';
import './App.css'; // Assuming you have CSS files in your project
import 'bootstrap/dist/css/bootstrap.min.css'; 
import BannerSection from './BannerSection'; 
function App() {
  return (
    <div id="outer">
      <header className="header order-last" id="tm-header">
        {/* Navigation section */}
      </header>

      <button className="navbar-button collapsed" type="button">
        {/* Navbar button */}
      </button>

      <main id="content-box" className="order-first">
        {/* Use BannerSection component */}
        <BannerSection />
        {/* Add your other components here */}
      </main>
    </div>
  );
}

export default App;

---------------------------------------------------------------------------------------------------------------------------------------------
// WorkSection
 
import React from 'react';

function WorkSection() {
  return (
    <section className="work-section section" id="section-2">
      <div className="container">
        <div className="row">
          <div className="item col-md-4">
            <div className="tm-work-item-inner">
              <div className="icn"><i className="fas fa-2x fa-icons"></i></div>
              <h3>.01 Get An Idea</h3>
              <p>Simply Amazed is free HTML template provided by Tooplate website. Please tell your friends about our website. Thank you.</p>
            </div>
          </div>
          <div className="item col-md-4 one">
            <div className="tm-work-item-inner">
              <div className="icn"><i className="fas fa-2x fa-tools"></i></div>
              <h3>.02 Create It</h3>
              <p>This is a full-width CSS template with bootstrap 5, you can download, modify and use this layout for your simple CSS website.</p>
            </div>
          </div>
          <div className="item col-md-4 two">
            <div className="tm-work-item-inner">
              <div className="icn">
                <i className="fab fa-2x fa-phoenix-framework"></i>
              </div>
              <h3>.03 Execute it</h3>
              <p>You are allowed to use this for your personal and commercial projects, you are not allowed to redistribute the template ZIP file on any download site.</p>
            </div>
          </div>
        </div>
        <div className="title">
          <h2>Our Work</h2>
        </div>
      </div>
    </section>
  );
}

export default WorkSection;

------------------------------------------------------------------------------------------------------------------------------------------------------------------
// App

import React from 'react';
import './App.css'; // Assuming you have CSS files in your project
import 'bootstrap/dist/css/bootstrap.min.css';
import WorkSection from './WorkSection'; 
function App() {
  return (
    <div id="outer">
      <header className="header order-last" id="tm-header">
        {/* Navigation section */}
      </header>

      <button className="navbar-button collapsed" type="button">
        {/* Navbar button */}
      </button>

      <main id="content-box" className="order-first">
        {/* Use WorkSection component */}
        <WorkSection />
        {/* Add your other components here */}
      </main>
    </div>
  );
}

export default App;

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
//GallerySection

import React from 'react';

function GallerySection() {
  return (
    <section className="gallery-section section parallax-window" data-parallax="scroll" data-image-src="img/section-3-bg.jpg" id="section-3">
      <div className="container">
        <div className="title text-right">
          <h2>Our Gallery</h2>
        </div>
        <div className="mx-auto gallery-slider">
          {/* Gallery images */}
          <figure className="effect-julia item">
            <img src="img/gallery-img-01.jpg" alt="Image" />
            <figcaption>
              <div>
                <p>Julia dances in the deep dark</p>
              </div>
              <a href="#">View more</a>
            </figcaption>
          </figure>
          <figure className="effect-julia item">
            <img src="img/gallery-img-02.jpg" alt="Image" />
            <figcaption>
              <div>
                <p>Julia dances in the deep dark</p>
              </div>
              <a href="#">View more</a>
            </figcaption>
          </figure>
          {/* Add more gallery images here */}
        </div>
      </div>
    </section>
  );
}

export default GallerySection;

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

//App

import React from 'react';
import './App.css'; // Assuming you have CSS files in your project
import 'bootstrap/dist/css/bootstrap.min.css'; 
import GallerySection from './GallerySection'; 
function App() {
  return (
    <div id="outer">
      <header className="header order-last" id="tm-header">
        {/* Navigation section */}
      </header>

      <button className="navbar-button collapsed" type="button">
        {/* Navbar button */}
      </button>

      <main id="content-box" className="order-first">
        {/* Use GallerySection component */}
        <GallerySection />
        {/* Add your other components here */}
      </main>
    </div>
  );
}

export default App;

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

import React from 'react';

function ContactSection() {
  return (
    <section className="contact-section section" id="section-4">
      <div className="container">
        <div className="title">
          <h3>Contact Us</h3>
        </div>
        <div className="row">
          <div className="col-lg-5 col-md-6 mb-4 contact-form">
            <div className="form tm-contact-item-inner">
              <form action="#" method="POST">
                <div className="form-group">
                  <input
                    name="name"
                    type="text"
                    className="form-control"
                    placeholder="Name"
                  />
                </div>
                <div className="form-group">
                  <input
                    name="email"
                    type="text"
                    className="form-control"
                    placeholder="Email"
                  />
                </div>
                <div className="form-group">
                  <textarea
                    name="message"
                    className="textarea form-control"
                    placeholder="Message"
                  ></textarea>
                </div>
                <div className="form-group text-right">
                  <input
                    type="submit"
                    className="btn btn-primary"
                    value="Send it"
                  />
                </div>
              </form>
            </div>
          </div>
          <div className="col-lg-4 col-md-6 mb-4 contact-details">
            <div className="tm-contact-item-inner-2">
              <p>
                Nam mollis felis elementum, placerat dolor id, vehicula
                libero. Etiam dui nisl, mattis ut rhoncus et, cursus ut
                diam.
              </p>
              <ul className="font-weight-light">
                <li>
                  <span className="icn"><i className="fas fa-mobile-alt"></i></span>
                  <span className="lbl">Tel:</span> <a href="#">010-020-0340</a>
                </li>
                <li>
                  <span className="icn"><i className="fas fa-at"></i></span>
                  <span className="lbl">Email:</span>
                  <a href="#">info@company.com</a>
                </li>
                <li>
                  <span className="icn"><i className="fas fa-globe-asia"></i></span>
                  <span className="lbl">URL:</span>
                  <a href="#">www.company.com</a>
                </li>
              </ul>
            </div>
          </div>
          <div className="col-lg-3 col-md-12 map">
            {/* Map */}
            <div className="map-outer tm-mb-40">
              <div className="gmap-canvas">
                <iframe
                  width="100%"
                  height="400"
                  id="gmap-canvas"
                  src="https://maps.google.com/maps?q=Av.+L%C3%BAcio+Costa,+Rio+de+Janeiro+-+RJ,+Brazil&t=&z=13&ie=UTF8&iwloc=&output=embed"
                  frameBorder="0"
                  scrolling="no"
                  marginHeight="0"
                  marginWidth="0"
                ></iframe>
              </div>
            </div>
          </div>
        </div>
      </div>
      <footer className="footer container container-2">
        <div className="row">
          <p className="col-sm-7">Copyright 2024 Dileep</p>
        </div>
      </footer>
    </section>
  );
}

export default ContactSection;

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
//App

import React from 'react';
import './App.css'; // Assuming you have CSS files in your project
import 'bootstrap/dist/css/bootstrap.min.css'; 
import ContactSection from './ContactSection'; 

function App() {
  return (
    <div id="outer">
      <header className="header order-last" id="tm-header">
        {/* Navigation section */}
      </header>

      <button className="navbar-button collapsed" type="button">
        {/* Navbar button */}
      </button>

      <main id="content-box" className="order-first">
        {/* Use ContactSection component */}
        <ContactSection />
        {/* Add your other components here */}
      </main>
    </div>
  );
}

export default App;

-------------------------------------------------------------------------------------------------------------------------

//Footer

import React from 'react';

function Footer() {
  return (
    <footer className="footer container container-2">
      <div className="row">
        <p className="col-sm-7">Copyright 2024 Prakhar</p>
      </div>
    </footer>
  );
}

export default Footer;

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------


//App

import React from 'react';
import './App.css'; // Assuming you have CSS files in your project
import 'bootstrap/dist/css/bootstrap.min.css'; 
import ContactSection from './ContactSection'; 
function App() {
  return (
    <div id="outer">
      <header className="header order-last" id="tm-header">
        {/* Navigation section */}
      </header>

      <button className="navbar-button collapsed" type="button">
        {/* Navbar button */}
      </button>

      <main id="content-box" className="order-first">
        {/* Use ContactSection component */}
        <ContactSection />
        {/* Add your other components here */}
      </main>
    </div>
  );
}

export default App;

-----------------------------------------------------------------------------------------------------------------------------------------------------------------

