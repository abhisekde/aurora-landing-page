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
<p style="font-family:arial;">Downloading your prescription...</p>
<iframe id="pdfView" />
