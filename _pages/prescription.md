---
title: Prescription
include_in_header: false
---
<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/2.16.105/pdf.min.js" integrity="sha512-tqaIiFJopq4lTBmFlWF0MNzzTpDsHyug8tJaaY0VkcH5AR2ANMJlcD+3fIL+RQ4JU3K6edt9OoySKfCCyKgkng==" crossorigin="anonymous" referrerpolicy="no-referrer">
</script>
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
<!-- <iframe id="pdfView" style="width: 100%; height: 100%; overflow: scroll; margin: 0; padding: 0; border: none;"/> -->
<iframe 
        title="Prescription" 
        src={`/pdfjs-2/web/viewer.html?file=${redirectUrl}`} 
        width=100% 
        height=00%
        ></iframe>
<!-- <embed id="pdfView" type="application/pdf" width="100%" height="100%"> -->
