---
title: Prescription
include_in_header: false
---
<script>
    // window.onload = function redirect() {
    var redirectUrl = '';
    function redirect() {
        redirectUrl = 'https://asia-south1-aurora-clinic-app.cloudfunctions.net/prescription?';
        var queryString = window.location.href.split('?')[1];
        if(queryString != null && queryString != undefined) {
            redirectUrl = redirectUrl + queryString; 
            // document.getElementById('pdfView').src = '/pdfjs-2/web/viewer.html?file=' +redirectUrl;
        } else {
            window.location = 'https://auroraclinic.app/';
        }
    }
    
    redirect();
    var pdfViewSrc = '/pdfjs-2/web/viewer.html?file=' +redirectUrl;
    
</script>
<!-- <iframe id="pdfView" style="width: 100%; height: 100%; overflow: scroll; margin: 0; padding: 0; border: none;"/> -->
<iframe 
        id="pdfView" 
        src=pdfViewSrc
        title="Prescription" 
        width="100%" 
        height="100%" 
        frameborder="0" >
</iframe>
<!-- <embed id="pdfView" type="application/pdf" width="100%" height="100%"> -->
