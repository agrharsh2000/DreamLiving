<template>
<div class="header-class">
    <div class="left">
        <h1>Let's Build <br><span>Your ____</span> Dream House</h1>

        <div class="button-container">
            <Button text="Find Property" @click="handleButtonClick" variant="primary" />
            <Button text="Explore" @click="handleButtonClick" variant="secondary" />
        </div>
        <div class="stacks-wrapper">
            <div class="stack">
                <span class="stack-heading">43K+</span>
                <span class="stack-description">Regular Customers</span>
            </div>
            <div class="stack">
                <span class="stack-heading">203K+</span>
                <span class="stack-description">Projects Completed</span>
            </div>
        </div>

    </div>
    <div class="right"></div>
</div>
</template>

<script>
export default {
    name: "Header",
}
</script>

<style scoped>
.header-class {
    margin-left: 40px;
}

.left {
    margin-top: 120px;
    margin-left: 26px;
    font-size: 40px;

}

h1 {

    text-align: left;

}

h1 span {
    display: block;
    margin-bottom: 20px;
}

.my-button {

    padding-left: 26px;
    padding-right: 26px;
    padding-top: 18px;
    padding-bottom: 18px;
    font-size: 26px;
    font-weight: 400;
    border-radius: 99px;
    border: none;
    transition: all 0.3s ease;

}

.my-button--primary {
    background-color: #000000;
    color: #ffffff;

}

.my-button:hover {
    background-color: #ffffff;
    color: #000000;

}

.my-button--secondary {
    background-color: #ffffff;
    color: #000000;
    padding-left: 50px;
    padding-right: 50px;
    margin-left: 10px;
    border: 1px solid;
}

.my-button:hover {
    background-color: #000000;
    color: #ffffff;
}

.stacks-wrapper {

    margin-top: 40px;
    display: flex;
    justify-content: space-between;
    gap: 10px;
    text-align: left;
}

.stack {
    display: flex;
    flex-direction: column;
}

.stack-heading {
    font-size: 40px;
    color: #EA6F4B;
}

.stack-description {
    font-size: 17px;

}
</style>
