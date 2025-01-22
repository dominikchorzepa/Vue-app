<template>
  <header>
        <div class="header-content">
            <div class="logged-in">
                <span>Zalogowany: <strong>Jan Kowalski</strong></span>
            </div>
            <div class="title">
                <h1>System Koła Myśliwskiego</h1>
                <h2>Administrator</h2>
            </div>
        </div>
    </header>

    <main>
        <div class="main-container">
            <div class="card" id="manage-users">
                <a href="#" class="card-link">Zarządzaj Użytkownikami</a>
            </div>
            <div class="card" id="add-hours">
                <a href="#" class="card-link">Dodaj Przepracowane Godziny</a>
            </div>
            <div class="card" id="set-limits">
                <a href="#" class="card-link">Ustal Limity</a>
            </div>
        </div>
    </main>

</template>

<script>
export default {

}
</script>

<style>
header {
    background-color: #4e5b31;  
    color: #fff;
    padding: 20px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;  
    height: 200px;  
}

.logged-in {
    font-size: 16px;
    position: absolute;
    top: 20px;
    left: 20px;
}

.title {
    position: absolute;  
    top: 50%;  
    left: 50%;  
    transform: translate(-50%, -50%); 
    text-align: center;
}

.title h1 {
    font-size: 36px;
    margin: 10px 0;
}

.title h2 {
    font-size: 24px;
    margin: 10px 0;
}

main {
    padding: 40px 20px;
}

.main-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
}

.card {
    width: 300px;
    height: 150px;
    background-color: #8c9e57;  
    border-radius: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: background-color 0.3s ease, transform 0.2s ease;
}

.card:hover {
    background-color: #a4b85f;  
    transform: scale(1.05);
}

.card-link {
    text-decoration: none;
    color: #fff;
    font-size: 18px;
    font-weight: bold;
}

@media (max-width: 768px) {
    .header-content {
        flex-direction: column;
        text-align: center;
    }

    .title h1 {
        font-size: 28px;
    }

    .title h2 {
        font-size: 18px;
    }

    .main-container {
        padding-top: 20px;
    }

    .card {
        width: 80%;
    }
}
</style>