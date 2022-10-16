---
title: Prescription
include_in_header: false
---
<script
    src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/2.0.943/pdf.min.js">
</script>
<script>
    window.onload = function redirect() {
        var redirectUrl = 'https://asia-south1-aurora-clinic-app.cloudfunctions.net/prescription?';
        var queryString = window.location.href.split('?')[1];
        if(queryString != null && queryString != undefined) {
            redirectUrl = redirectUrl + queryString; 
            window.open(redirectUrl, 'fullscreen=yes')
        } else {
            window.location = 'https://auroraclinic.app/';
        }
    }
</script>
