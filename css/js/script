// =========================
// MARATHON COUNTDOWN
// =========================

const marathonDate = new Date("September 12, 2026 06:30:00").getTime();

const countdown = setInterval(function () {

    const now = new Date().getTime();

    const distance = marathonDate - now;

    const days = Math.floor(distance / (1000 * 60 * 60 * 24));

    const hours = Math.floor(
        (distance % (1000 * 60 * 60 * 24)) /
        (1000 * 60 * 60)
    );

    const minutes = Math.floor(
        (distance % (1000 * 60 * 60)) /
        (1000 * 60)
    );

    const seconds = Math.floor(
        (distance % (1000 * 60)) /
        1000
    );

    const daysElement = document.getElementById("days");
    const hoursElement = document.getElementById("hours");
    const minutesElement = document.getElementById("minutes");
    const secondsElement = document.getElementById("seconds");

    if (daysElement) {
        daysElement.innerHTML = days;
    }

    if (hoursElement) {
        hoursElement.innerHTML = hours;
    }

    if (minutesElement) {
        minutesElement.innerHTML = minutes;
    }

    if (secondsElement) {
        secondsElement.innerHTML = seconds;
    }

    if (distance < 0) {

        clearInterval(countdown);

        document.getElementById("countdown").innerHTML =
            "THE MARATHON IS ON!";

    }

}, 1000);
