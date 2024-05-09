<template>
  <div>
    <button @click="downloadPDF">download PDF</button>

  </div>
</template>


<script>
export default {
  name: 'DownloadPdfButton',
  props: {
    pdfUrl: {
      type: String,
      required: true
    },
    pdfFileName: {
      type: String,
      required: true
    }
  },
  methods: {
    downloadPDF(){
      const link = document.createElement('a');
      link.href = this.pdfUrl;
      link.target = '_blank';
      link.download = this.pdfFileName;

      document.body.appendChild(link);
      link.click();
      document.body.removeChild(link);
    }
  }
}

</script>