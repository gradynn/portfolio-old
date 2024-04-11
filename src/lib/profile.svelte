<style lang="scss">
    .container {
        height: 100vh;
        width: 100%;
        display: flex;
        flex-direction: row;
        color: color('primary');
    }
    
    .profile-section {
        height: 100vh;
        width: 50%;
        padding-top: 5rem;
        padding-bottom: 5rem;
        padding-left: 1rem;
        box-sizing: border-box;
    }
    
    .photo-section {
        display: flex;
        background-image: url('/me1.png');
        background-size: cover;
        background-position: left;
        filter: grayscale(1);
    }
    
    .info-section {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: left;
    }

    h1 {
        font-size: 4rem;
        border-bottom: 1px solid color('primary');
        width: fit-content;
    }

    .fa-envelope {
        font-size: 2rem;
        padding-right: 1rem;
    }

    .email {
        display: flex;
        align-items: center;
    }
    
    /* Removed img styles since we're now using background-image */
</style>
    
<div class="container">
    <div class="profile-section photo-section">
    </div>
    <div class="profile-section info-section">
        <h1>Gradyn Nagle</h1>
        <div class="email">
            <span class="material-icons">email</span>
            <h2>gnagle@ucdavis.edu</h2>
        </div>
    </div>
</div>