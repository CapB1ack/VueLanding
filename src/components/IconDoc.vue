<template>
  <div class="account-icons-wrapper">
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
      sodipodi:docname="my_doc.svg"
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
        inkscape:zoom="5.37"
        inkscape:cx="61.669507"
        inkscape:cy="27.600401"
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
            <dc:title />
          </cc:Work>
        </rdf:RDF>
      </metadata>
      <g
        inkscape:label="Layer 1"
        inkscape:groupmode="layer"
        id="layer1"
        transform="translate(0,-270.54167)">
        <rect
          style="fill:#333333;fill-opacity:1;stroke:#333330;stroke-width:0.05281107;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          id="rect4744"
          width="26.405521"
          height="26.405552"
          x="0.026392339"
          y="270.56818" />
        <rect
          style="fill:#ffffff;fill-opacity:1;stroke:#333330;stroke-width:0.05339054;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          id="rect4722"
          :class="{'hovered': hovered}"
          class="hoverable"
          width="21.113276"
          height="26.404943"
          x="2.6725285"
          y="270.56836" />
        <rect
          style="fill:#333333;fill-opacity:1;stroke:#333330;stroke-width:0.02857826;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          id="rect4724"
          width="9.260416"
          height="7.9374866"
          x="15.875"
          y="289.0625" />
        <path
          style="fill:#ffffff;fill-opacity:1;stroke:#333330;stroke-width:0.05291667;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          d="m 17.197916,290.38541 h 5.291667 l -5.291667,5.29167 z"
          id="rect4726"
          :class="{'hovered': hovered}"
          class="hoverable"
          inkscape:connector-curvature="0"
          sodipodi:nodetypes="cccc" />
        <rect
          style="fill:#333333;fill-opacity:1;stroke:#333330;stroke-width:0.05291667;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          id="rect4746"
          width="15.875"
          height="2.6458333"
          x="5.2916665"
          y="273.1875" />
        <rect
          style="fill:#333333;fill-opacity:1;stroke:#333330;stroke-width:0.05291667;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          id="rect4748"
          width="13.229166"
          height="2.6458333"
          x="5.2916665"
          y="278.47916" />
      </g>
    </svg>
  </div>
</template>
<script>
  export default {
    name: 'IconDoc',
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
