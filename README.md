import Replicate from 'replicate';
const replicate = new Replicate();

const input = {
    image: "https://replicate.delivery/pbxt/KW7Getr2zD5ECxySdBZtLmPa322lNkXrpkMdKcmxeaDmq2b1/MTk4MTczMTkzNzI1Mjg5NjYy.webp",
    style: "Clay",
    prompt: "a person in a post apocalyptic war game",
    instant_id_strength: 0.8
};

const output = await replicate.run("fofr/face-to-many:352f1ad684b6e7e6d5c0895a73dde3bf22131ebdc4a2b17aa3a64e7c2aa40d96", { input });
console.log(output)
//=> ["https://replicate.delivery/pbxt/R1ayGe5efoQbaoRzgDEJdLs...
