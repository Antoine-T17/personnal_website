document.addEventListener("DOMContentLoaded", function() {
  const animatedElements = document.querySelectorAll('.slide-in-left, .slide-in-right, .fade-in');

  const observer = new IntersectionObserver((entries, observer) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('in-view');
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.5 });

  animatedElements.forEach(el => {
    observer.observe(el);
  });
});
