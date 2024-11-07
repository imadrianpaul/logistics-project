<script>

    import {FaArrowRight} from "svelte-icons/fa";
    import {FaTruck} from "svelte-icons/fa";

</script>

<section class="hero-section">
    <div class="hero-spacing">

    </div>
    <div class="hero-content">
        <h1 class="hero-title">Your Easiest <br>
            Way to Deliver</h1>
        <p class ="hero-desc">uParcel offers on-demand delivery and courier services for business and consumers. <br>
            Be it a document, small parcel or bulky goods, we will get them delivered.</p>
        <div class="button-container">
            <button class="book-delivery-button">
                <div class="button-text">Book Delivery</div>
                <div class="circle-icon">
                    <svg>
                        <FaArrowRight />
                    </svg>
                </div>
            </button>
        </div>
    <div class="hero-spacing2">

    </div>

        <div class="track-container">
            <div class="tracking">
                <svg class="truck-icon">
                <FaTruck />
                </svg>
                <span class="track-text">Track Your parcel</span>
            </div>
            <input type="text" class="track-input" placeholder="Enter your tracking code" />
            <button class="track-button">
                <div class="track-button-text">Track
                </div>
            </button>
        </div>
    </div>
</section>

<style>
    .hero-section {
        display: flex;
        flex-direction: column;
        justify-content: center;
        height: 100vh;
        text-align: center;
        background-color: transparent;
        padding: 2rem;
        background-size: cover;
    }

    .hero-spacing {
        margin: 4rem;
        padding: 3rem;

    }

    .hero-content {
        background-color: transparent;
        z-index: 2;
    }

    .hero-title {
        font-size: 96px;
        margin: 2rem 0;
        padding-top: 2rem;
        color: #333;
        text-transform: uppercase;
        font-family: Unbounded, sans-serif;

        background: linear-gradient(90deg, rgba(255, 255, 255, 1), rgba(254, 162, 56, 1));
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent
        
    }

    .hero-desc {
        font-size: 24px;
        margin: 1rem 0;
        color: #ffffff;
    }

    .button-container {
        display: inline-block;
    }

    .book-delivery-button {
        position: relative;
        padding-right: 5rem;
        margin: 4rem;
        height: 75px;
        background-color: #fea238;
        color: rgb(255, 255, 255);
        border: none;
        border-radius: 50px;
        cursor: pointer;       
        transition: background-color 0.3s ease;
    }

    .button-text {
        padding: 0.75rem;
        font-size: 24px;
        text-align: center;
        text-transform: uppercase;
        font-family: Unbounded, sans-serif;
    }

    .circle-icon {
        position: absolute;
        right: -10px;
        top:50%;
        transform: translateY(-50%);
        width: 70px;
        height: 70px;
        color: rgb(127, 91,23);
        background-color: #ffffff;
        border-radius: 50%;
        border: 5px solid rgb(127, 91,23);
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .book-delivery-button:hover {
        background-color: #0056b3;
    }


    .hero-spacing2 {
        margin: 2rem;
        padding: 2rem;
    }

    /* Track Part Styling */

    .track-container {
        justify-content: center;
        align-items: center;
        padding-top: 4rem;
        position: relative;
        bottom: 0;

    }

    .tracking {
        
        margin-right: 0.5rem;
        padding-top: 1rem;
        padding-bottom: 2.5rem;
        color: rgb(127, 91,23);
        height: 24px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .truck-icon {

        margin-right: 1rem;  
        margin-bottom: 0.75rem;      

    }

    .track-text {
        padding-bottom: 1rem;
        font-size: 24px;
        font-weight: bold;
        text-transform: uppercase;
        color: #fff;
    }
    
    .track-button-text {
        font-size: 24px;
        font-family: Unbounded, sans-serif;
        text-align: center;
        text-transform: uppercase;
    }

    .track-input {

        padding: 0.75rem 2.5rem;
        font-size: 16px;
        border: 2px solid #ccc;
        border-radius: 40px;
        outline: none;
        height: 44px;
        width: 500px;
    }

    .track-button {
        
        padding: 0 4rem;
        margin: 1rem;
        height: 75px;
        justify-content: center;
        align-items: center;
        background-color: #fea238;
        color: #fff;
        border: none;
        border-radius: 50px;
        cursor: pointer;
        transition: background-color 0.3s ease;
    }

    .track-text {
        text-align: center;
    }

    .track-button:hover {
        background-color: #0056b3;
    }
</style>