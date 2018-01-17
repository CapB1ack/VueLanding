<template>
  <div  class="account-icons-wrapper">
    <svg
      @mouseenter="handleMouse(true)"
      @mouseleave="handleMouse(false)"
      xmlns:dc="http://purl.org/dc/elements/1.1/"
      xmlns:cc="http://creativecommons.org/ns#"
      xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
      xmlns:svg="http://www.w3.org/2000/svg"
      xmlns="http://www.w3.org/2000/svg"
      xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd"
      xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape"
      width="100%"
      height="100%"
      viewBox="0 0 26.458333 26.458333"
      version="1.1"
      id="svg3747"
      sodipodi:docname="my_phone.svg"
      inkscape:version="0.92.1 r15371">
      <defs
        id="defs3741" />
      <sodipodi:namedview
        id="base"
        pagecolor="#ffffff"
        bordercolor="#666666"
        borderopacity="1.0"
        inkscape:pageopacity="0.0"
        inkscape:pageshadow="2"
        inkscape:zoom="3.7971634"
        inkscape:cx="-8.8971793"
        inkscape:cy="51.092324"
        inkscape:document-units="mm"
        inkscape:current-layer="layer1"
        showgrid="true"
        units="px"
        inkscape:measure-start="-44.2436,97.1778"
        inkscape:measure-end="0,0"
        showguides="false"
        inkscape:window-width="1366"
        inkscape:window-height="706"
        inkscape:window-x="-8"
        inkscape:window-y="-8"
        inkscape:window-maximized="1">
        <inkscape:grid
          type="xygrid"
          id="grid4590" />
      </sodipodi:namedview>
      <metadata
        id="metadata3744">
        <rdf:RDF>
          <cc:Work
            rdf:about="">
            <dc:format>image/svg+xml</dc:format>
            <dc:type
              rdf:resource="http://purl.org/dc/dcmitype/StillImage" />
            <dc:title></dc:title>
          </cc:Work>
        </rdf:RDF>
      </metadata>
      <g
        inkscape:label="Layer 1"
        inkscape:groupmode="layer"
        id="layer1"
        transform="translate(0,-270.54167)">
        <rect
          style="fill:#ffffff;fill-opacity:1;stroke:#333333;stroke-width:0.0912329;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          id="rect4805"
          :class="{'hovered': hovered}"
          class="hoverable"
          width="15.783767"
          height="26.3671"
          x="5.3372831"
          y="270.58728"
          ry="2.594533" />
        <rect
          style="fill:#333330;fill-opacity:1;stroke:#333333;stroke-width:0.09354436;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          id="rect4807"
          width="13.229167"
          height="19.843756"
          x="6.6145835"
          y="273.1875" />
        <path
          style="fill:#333333;fill-opacity:1;stroke:#333333;stroke-width:0.09667555;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          d="m 10.52905,294.34937 c 2.009229,10e-6 4.018459,10e-6 5.479717,0 0.304426,0 0.304426,1.33249 0,1.33249 -1.461258,2e-5 -3.470488,2e-5 -5.479717,0 -0.304423,0 -0.304423,-1.33249 0,-1.33249 z"
          id="rect4809"
          inkscape:connector-curvature="0"
          sodipodi:nodetypes="sssss" />
      </g>
    </svg>

  </div>
</template>
<script>
  export default {
    name: 'IconGauge',
    data () {
      return {
        hovered: false
      }
    },
    methods: {
      handleMouse (flag) {
        this.hovered = flag
      }
    }
  }
</script>
<style lang="stylus">

</style>
