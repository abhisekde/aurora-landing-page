---
layout: page
title: Prescription
include_in_header: false
---
<script>
    var queryString = window.location.href.split('?')[1];
    if(queryString != null && queryString != undefined) {
        window.location = 'https://asia-south1-aurora-clinic-app.cloudfunctions.net/prescription?' + queryString; 
    } else {
        window.location = 'https://auroraclinic.app/';
    }
</script>
