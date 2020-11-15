for rightsideBar for a page:

<div class="has-sidebar">

    <!-- right sidebar -->


    <!--  left side-->
    <div class="left-sidebar">
        <!-- insert leftside here -->
    </div>
    <!-- end of left side-->

</div>

and add this script to open clicked collapse and close other ones:

<script>
    $( document ).ready(function() {
        $('.collapse').on('show.bs.collapse', function () {

        // hide all accordion except the clicked one
        $('.collapse').not(this).collapse('hide');
        
        });
    });
</script>
