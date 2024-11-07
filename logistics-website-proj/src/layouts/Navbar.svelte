<script>

    import { FaUser } from "svelte-icons/fa";

</script>

<nav class="nav-bar">
    <ul class="nav-links">
        <li>
            <a href="*">
            <img src="/src/assets/logo.png" alt="uParcel Logo" class="logo" />
        </a>
        <li><a href="#services">Services</a></li>
        <li><a href="#how-it-works">How It Works?</a></li>
        <li><a href="#tracking">Tracking</a></li>
        <li><a href="#faqs">FAQs</a></li>
        <li><a href="#rates">Rates</a></li>
        <li><a href="#contact-us">Contact Us</a></li>
        <li>
            <button class="sign-up-button">
                <svg class="user-icon">
                <FaUser />
                </svg>
                <span>Sign Up / Login</span>
            </button>
        </li>
    </ul>
</nav>

<style>
    .nav-bar {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        background-color: transparent;
        justify-content: space-between;
        align-items: center;
        margin: 1rem 4rem;
        padding: 1rem 8rem;
        z-index: 1000;
        justify-content: center;
        font-size: 20px;
        text-transform: uppercase;
    }
    
    .nav-links {
        list-style: none;
        display: flex;
        margin: 0 4rem;
        padding: 0.5rem 4rem;
        gap: 1.75rem;
        justify-content: center;
        align-items: center;
    }

    .nav-links li a {
        text-decoration: none;
        color: #ffffff;
        transition: color 0.3s ease;
        font-weight: 500;
        font-family: Inter, sans-serif;
    }

    .nav-links li a:hover {
        color: #007BFF;
    }

    .sign-up-button {
        padding: 0 2rem;
        margin: 1rem;
        height: 75px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #fea238;
        color: #fff;
        border: none;
        border-radius: 50px;
        cursor: pointer;
        transition: background-color 0.3s ease;
        font-weight: 500; 
        font-size: 20px; 
        font-family: Inter, sans-serif;
        text-transform: uppercase;
    }

    .user-icon {
        margin-right: 1rem; /* Space between icon and text */
        margin-top: 0.25rem;
        padding-bottom: 0.25rem;
    }

    @media (max-width: 768px) {

        .nav-bar {
        padding: 1rem;
        flex-direction: column;
        background-color: #333; /* Set a solid color background for readability */
        }

        .nav-links {
        flex-direction: column;
        gap: 1rem;
        }

        .sign-up-button {
        width: 100%;
        height: 50px;
        font-size: 16px;
        padding: 0.5rem 1rem;
        }

    }

    /* Mobile Layout */
    @media (max-width: 480px) {
        
        .nav-bar {
            padding: 0.5rem;
        }

        .nav-links {
            gap: 0.5rem;
            font-size: 16px;
        }

        .sign-up-button {
            font-size: 14px;
            padding: 0.5rem 1rem;
        }

        .nav-links li a {
            font-size: 14px;
        }
    }

</style>