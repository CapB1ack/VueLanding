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
      sodipodi:docname="my_plus.svg"
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
        inkscape:zoom="2.685"
        inkscape:cx="58.868533"
        inkscape:cy="16.761868"
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
        <circle
          style="fill:#ffffff;fill-opacity:1;stroke:#333330;stroke-width:0.0681392;stroke-linecap:round;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
          id="path4750"
          :class="{'hovered': hovered}"
          class="hoverable"
          cx="13.229167"
          cy="283.77081"
          r="13.195097" />
        <path
          style="fill:none;stroke:#333333;stroke-width:0.52916667;stroke-linecap:butt;stroke-linejoin:miter;stroke-opacity:1;stroke-miterlimit:4;stroke-dasharray:none"
          d="m 13.229167,270.54167 c 0,26.45833 0,26.45833 0,26.45833"
          id="path4752"
          inkscape:connector-curvature="0" />
        <path
          style="fill:none;stroke:#333333;stroke-width:1.32291667;stroke-linecap:round;stroke-linejoin:miter;stroke-opacity:1;stroke-miterlimit:4;stroke-dasharray:none"
          d="m 15.875,283.77084 c 7.9375,0 7.9375,0 7.9375,0"
          id="path4773"
          inkscape:connector-curvature="0" />
        <path
          style="fill:none;stroke:#333333;stroke-width:1.32291667;stroke-linecap:round;stroke-linejoin:miter;stroke-opacity:1;stroke-miterlimit:4;stroke-dasharray:none"
          d="m 2.6458333,283.77084 c 7.9374997,0 7.9374997,0 7.9374997,0"
          id="path4775"
          inkscape:connector-curvature="0" />
        <path
          style="fill:none;stroke:#333333;stroke-width:1.32291667;stroke-linecap:round;stroke-linejoin:miter;stroke-opacity:1;stroke-miterlimit:4;stroke-dasharray:none"
          d="m 6.6145832,279.80209 c 0,7.9375 0,7.9375 0,7.9375"
          id="path4777"
          inkscape:connector-curvature="0" />
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
