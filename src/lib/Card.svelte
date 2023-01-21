<script>
    export let item, index;

    let colors = [
        "rgb(4, 113, 255, 0.1)",
        "rgb(207, 0, 255, 0.1)",
        "rgb(255, 118, 0, 0.1)",
        "rgba(2, 185, 76, 0.1)"
    ]
</script>

<div class="card-wrapper">
    <div style="background-color: {colors[index]};" class="card-icon">
        <img src={item.icon} alt="" />
    </div>
    <div class="card-label">
        <h3>{item.label}</h3>
    </div>
    <div class="card-description">
        {item.description}
    </div>
</div>

<style>
    .card-wrapper {
        background-color: rgb(255, 255, 255);
        transition: .3s;
        margin: 20px;
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        gap: 1.5rem;
        padding: 2rem;
        border-radius: 1em;
        height: fit-content;
    }
    
    .card-wrapper:hover {
        -webkit-box-shadow: 3px 3px 13px 3px rgba(235, 235, 235, 1);
        -moz-box-shadow: 3px 3px 13px 3px rgba(235, 235, 235, 1);
        box-shadow: 3px 3px 13px 3px rgba(235, 235, 235, 1);
    }

    .card-wrapper .card-icon {
        height: 100px;
        display: flex;
        align-items: center;
        justify-content: center;
        aspect-ratio: 1/1;
        width: fit-content;
        border-radius: 50%;
    }
</style>
