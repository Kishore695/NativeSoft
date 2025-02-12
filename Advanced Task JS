// Add interactivity to the CTA button
document.getElementById("ctaButton").addEventListener("click", () => {
    alert("Thank you for your interest! We'll be in touch soon.");
  });
  
  // Expand blog post summaries
  const readMoreButtons = document.querySelectorAll(".btn");
  
  readMoreButtons.forEach(button => {
    button.addEventListener("click", (e) => {
      e.preventDefault();
      const post = e.target.closest(".post");
      const summary = post.querySelector("p");
      summary.classList.toggle("expanded");
      e.target.textContent = summary.classList.contains("expanded") ? "Read Less" : "Read More";
    });
  });
  
  // Lazy loading images
  document.addEventListener("DOMContentLoaded", () => {
    const lazyImages = document.querySelectorAll("img[data-src]");
  
    const lazyLoad = () => {
      lazyImages.forEach(img => {
        if (img.getBoundingClientRect().top < window.innerHeight) {
          img.src = img.dataset.src;
          img.removeAttribute("data-src");
        }
      });
    };
  
    window.addEventListener("scroll", lazyLoad);
    lazyLoad(); // Load images on page load
  });
