---
title: Prescription
include_in_header: false
---
<script>
    window.onload = function redirect() {
        var redirectUrl = 'https://asia-south1-aurora-clinic-app.cloudfunctions.net/prescription?';
        var queryString = window.location.href.split('?')[1];
        if(queryString != null && queryString != undefined) {
            redirectUrl = redirectUrl + queryString; 
            document.getElementById('pdfView').src = redirectUrl;
        } else {
            window.location = 'https://auroraclinic.app/';
        }
    }
</script>
<embed id="pdfView" type="application/pdf" width="100%" height="100%">
