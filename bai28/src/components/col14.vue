<template>
    <div v-bind:class="class">
        <h1>{{ head1 }}</h1>
        <p>{{ message }}
        </p>
        <button>{{ button }}</button>
    </div>
</template>
<script>
export default {


    prop [
        {
            class: 'col1',
            head1: 'A Elegant Design',
            message: 'Bacon ipsum dolor sit amet meatball shank park chop capicola fatback park loin sirloin flank. <b>Andouille</b> tongue corned beef rump pork loin shnk meatball capicola turducken venison shankle kevin pancetta tri-tip boudin.',
            button: 'BLUE BUTTON WITH MODAL VIDEO'

        },
        {
            class: 'col4',
            head1: 'Pretty easy to customize',
            message: 'Bacon ipsum dolor sit amet meatball shank park chop capicola fatback park loin sirloin flank.<b>Andouille</b> tongue corned beef rump pork loin shnk meatball capicola turducken venison shankle kevin pancetta tri-tip boudin.',
            button: 'ANOTHER BUTTON'
        }
    ]
        
        
    }
</script>
<style></style>

