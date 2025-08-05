// Fermer la bannière de bienvenue
function closeWelcome() {
    document.getElementById('welcomeBanner').style.display = 'none';
}

// Gestion du panier
document.addEventListener('DOMContentLoaded', function() {
    let cartCount = 0;
    const cartCountElement = document.querySelector('.cart-count');
    const addToCartButtons = document.querySelectorAll('.add-to-cart');
    
    // Ajouter un produit au panier
    addToCartButtons.forEach(button => {
        button.addEventListener('click', function() {
            cartCount++;
            cartCountElement.textContent = cartCount;
            
            // Animation du bouton
            this.textContent = 'Ajouté !';
            this.style.backgroundColor = '#2ecc71';
            
            setTimeout(() => {
                this.textContent = 'Ajouter au panier';
                this.style.backgroundColor = '#3498db';
            }, 1500);
            
            // Vous pouvez ajouter ici la logique pour stocker les articles dans le panier
        });
    });
    
    // Menu mobile (pour une future implémentation)
    const menuToggle = document.querySelector('.menu-toggle');
    const navLinks = document.querySelector('.nav-links');
    
    if (menuToggle) {
        menuToggle.addEventListener('click', function() {
            navLinks.classList.toggle('active');
        });
    }
    
    // Smooth scrolling pour les ancres
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function(e) {
            e.preventDefault();
            
            const targetId = this.getAttribute('href');
            if (targetId === '#') return;
            
            const targetElement = document.querySelector(targetId);
            if (targetElement) {
                window.scrollTo({
                    top: targetElement.offsetTop - 80,
                    behavior: 'smooth'
                });
            }
        });
    });
});

// Fonctionnalité de défilement pour révéler l'en-tête
let lastScroll = 0;
window.addEventListener('scroll', function() {
    const currentScroll = window.pageYOffset;
    const header = document.querySelector('header');
    
    if (currentScroll <= 0) {
        header.style.boxShadow = '0 2px 10px rgba(0, 0, 0, 0.1)';
        return;
    }
    
    if (currentScroll > lastScroll) {
        // Défilement vers le bas
        header.style.transform = 'translateY(-100%)';
        header.style.boxShadow = 'none';
    } else {
        // Défilement vers le haut
        header.style.transform = 'translateY(0)';
        header.style.boxShadow = '0 2px 10px rgba(0, 0, 0, 0.1)';
    }
    
    lastScroll = currentScroll;
});