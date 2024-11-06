<script>

    import Cards from "../../components/HomePage/Cards.svelte";
    import Features from "../../components/HomePage/Features.svelte";

    </script>

<section class="s-d-f-section">
    <div class="services-content">
        <h2 class="services-title-main">Services</h2>
        <div class="services-columns">
            <div class="services-item">
                <h3 class="services-title">Delivery and Courier of Documents and Packages</h3>
                <p class="services-desc">uParcel provides door-to-door delivery services for up to 25kg per carton, max of 200 cm (H+L+W). <br><br> No minumum quantity is required.</p>
            </div>
            <div class="services-item">
                <h3 class="services-title">Delivery Heavy and Bulky Goods</h3>
                <p class="services-desc">uParcel provides Vans, MPV and Lorries to help you with your bluky and high volume of goods. <br><br> Manpower for moving is also available if required.</p>
            </div>
            <div class="services-item">
                <h3 class="services-title">Warehouse / E-Fulfillment</h3>
                <p class="services-desc">uParcel provides a range of storage solutions including in Aircon and Ambient conditions. <br><br> We also help customers in their pick and pack for B2B and B2C orders.</p>
            </div>
        </div>
    <div class="delivery-content">
        <h2 class="delivery-title-main">Delivery Types</h2>
        <div class="delivery-columns">
            <div class="delivery-cards">

                <Cards
                    title="Specific Time"
                    subtitle="With Min. Order"
                    description="Delivery by a specific time +/- 20 minutes"
                    description2="Last cut-off time: 7:00 PM"
                >
                    <button slot="actions" class="card-button">From $13</button>
                </Cards>

                <Cards
                title="Same Day"
                subtitle="With Min. Order"
                description="Pick-up and Delivery in 6 hours"
                description2="Last cut-off time: 5:00 PM & For delivery: 11:00 PM"
                >
                <button slot="actions" class="card-button">From $13</button>
                </Cards>

                <Cards
                title="1 Hour Rush"
                subtitle="With Min. Order"
                description="Pick-up and Delivery in 1 hour"
                description2="Last cut-off time: 7:00 PM"
                >
                <button slot="actions" class="card-button">From $13</button>
                </Cards>

                <Cards
                title="Lorry Service"
                subtitle="With Min. Order"
                description="Delivery via 3 hours express / Specific time service"
                >
                <button slot="actions" class="card-button">From $13</button>

                </Cards>

            </div>
        </div>
    </div>
    <div class="features-content">
        <h2 class="features-title-main">Features</h2>
        <div class="features-columns">
            <div class="features-item">

                <Features
                title="Transparent Flat Rates from $7"
                icon=""
                description="Flat rates regardless of distance. Contact us for further discount if you have bulk deliveries."
                >       
                </Features>

                <Features
                title="Corporate Account"
                icon=""
                description="Monthly billing for corporate users. Create multiple sub-accounts for various business units."
                >       
                </Features>

                <Features
                title="Fixed Fleet for Regular Deliveries"
                icon=""
                description="Create your own team of delivery agents digital signatures, photos"
                >       
                </Features>

            </div>
            <div class="features-item">

                <Features
                title="Fast and Affordable with no Minimum Deliveries"
                icon=""
                description="Pre-paid E-wallet can be used or withdrawn anytime within 12 months make booking even for 1 parcel."
                >       
                </Features>

                <Features
                title="Track"
                icon=""
                description="Whatsapp and Email notifications to your receivers with expected delivery date and time. Proof of delivery report provided."
                >       
                </Features>

                <Features
                title="Batch Deliveries"
                icon=""
                description="Bulk excel file upload for multiple locations. Discounts up to 50% for deliveries going to the same location."
                >       
                </Features>

            </div>        
        </div>
    </div>

</section>

<style>

    .s-d-f-section {
        display: grid;
        grid-template-columns: 1fr;
        gap: 2rem;
        padding: 2rem;
    }

    .services-content {

        margin: 0 10rem;
    }

    .services-columns {

        display: flex;
        grid-template-columns: repeat(3, 1fr);
        gap: 7.5rem;
        text-align: center;
        justify-content: center;
        margin: 0 2.5rem;
        padding: 0 2.5rem;

    }

    .services-item {
        margin: 0 1rem;
        padding: 0 1rem;
        justify-content: center;
        align-items: center;
        display:flexbox;
    }

    .services-title-main {

        font-size: 48px;
        color: #fea238;
        text-align: center;

    }

    .services-title {

        color: rgb(127, 91,23);
        font-size: 24px;
        height: 50px;
        width: 300px;

    }

    .services-desc {
        font-size: 16px;
        font-family: Inter, sans-serif;
        height: 150px;
        width: 300px;
    }

    .delivery-content {
        text-align: center;
    }

    .delivery-title-main {

        font-size: 48px;
        color: #fea238;
        text-align: center;

    }

    .delivery-columns {
        text-align: center;
        justify-content: center;
        display: flex;
    }

    .delivery-cards {

        justify-content: center;
        display: grid;
        margin: 1rem;
        padding: 1rem;
        grid-template-columns: repeat(4, 1fr);
        gap: 2.5rem;


    }

    .features-title-main {

        font-size: 48px;
        color: #fea238;
        text-align: center;

    }

    .features-content {

        margin: 0 10rem;
        text-align: left;

    }

    .features-columns {

        justify-content: center;
        display: flex;
        grid-template-columns: repeat(2, 1fr);
        gap: 7.5rem;

    }

    .features-item {

        display: flex;
        flex-direction: column;
        gap: 1.5rem;
        
    }

    .features-description {

        font-size: 16px;
    }
   
</style>