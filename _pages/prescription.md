<script>
    var queryString = window.location.href.split('?')[1];
    if(queryString != null && queryString != undefined) {
        window.location = 'https://asia-south1-aurora-clinic-app.cloudfunctions.net/prescription?' + queryString; 
    } else {
        window.location = window.location.href.split('?')[0];
    }
</script>
