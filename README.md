css:
{
  "version": 1,
  "author": "Anonymous maker",
  "editor": "wokwi",
  "parts": [
    { "type": "wokwi-breadboard", "id": "bb1", "top": 45, "left": -64.4, "attrs": {} },
    {
      "type": "wokwi-arduino-uno",
      "id": "uno",
      "top": -239.4,
      "left": -0.6,
      "rotate": 180,
      "attrs": {}
    },
    {
      "type": "wokwi-pushbutton-6mm",
      "id": "btn1",
      "top": 173.8,
      "left": 157.6,
      "rotate": 90,
      "attrs": { "color": "green" }
    },
    {
      "type": "wokwi-pushbutton-6mm",
      "id": "btn2",
      "top": 173.8,
      "left": 272.8,
      "rotate": 90,
      "attrs": { "color": "green" }
    },
    {
      "type": "wokwi-pushbutton-6mm",
      "id": "btn3",
      "top": 173.8,
      "left": 388,
      "rotate": 90,
      "attrs": { "color": "green" }
    },
    {
      "type": "wokwi-pushbutton-6mm",
      "id": "btn4",
      "top": 173.8,
      "left": 493.6,
      "rotate": 90,
      "attrs": { "color": "green" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r1",
      "top": 273.6,
      "left": 133.85,
      "rotate": 90,
      "attrs": { "value": "10000" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r2",
      "top": 244.8,
      "left": 469.85,
      "rotate": 90,
      "attrs": { "value": "10000" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r3",
      "top": 235.2,
      "left": 354.65,
      "rotate": 90,
      "attrs": { "value": "10000" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r4",
      "top": 273.6,
      "left": 249.05,
      "rotate": 90,
      "attrs": { "value": "10000" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r5",
      "top": 99.95,
      "left": 412.8,
      "attrs": { "value": "200" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r6",
      "top": 99.95,
      "left": 182.4,
      "attrs": { "value": "200" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r7",
      "top": 99.95,
      "left": 518.4,
      "attrs": { "value": "200" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r8",
      "top": 99.95,
      "left": 297.6,
      "attrs": { "value": "200" }
    },
    {
      "type": "wokwi-buzzer",
      "id": "bz1",
      "top": 35.7,
      "left": 42.9,
      "rotate": 90,
      "attrs": { "volume": "0.1" }
    },
    {
      "type": "wokwi-led",
      "id": "led1",
      "top": 46.8,
      "left": 169.8,
      "rotate": 90,
      "attrs": { "color": "blue" }
    },
    {
      "type": "wokwi-led",
      "id": "led2",
      "top": 46.8,
      "left": 496.2,
      "rotate": 90,
      "attrs": { "color": "red" }
    },
    {
      "type": "wokwi-led",
      "id": "led3",
      "top": 46.8,
      "left": 285,
      "rotate": 90,
      "attrs": { "color": "cyan" }
    },
    {
      "type": "wokwi-led",
      "id": "led4",
      "top": 46.8,
      "left": 400.2,
      "rotate": 90,
      "attrs": { "color": "purple" }
    }
  ],
  "connections": [
    [ "btn1:2.r", "r1:1", "green", [ "v10.4", "h-19.6", "v38.4" ] ],
    [ "r1:2", "bb1:bn.17", "green", [ "h0" ] ],
    [ "btn1:1.r", "bb1:bp.19", "green", [ "v0" ] ],
    [ "r4:1", "btn2:2.r", "green", [ "h-9.6", "v-38.4", "h19.2" ] ],
    [ "r4:2", "bb1:bn.27", "green", [ "h9.6", "v-1.2" ] ],
    [ "btn2:1.r", "bb1:bp.29", "green", [ "v0" ] ],
    [ "btn3:2.r", "r3:1", "green", [ "v0" ] ],
    [ "r3:2", "bb1:bn.36", "green", [ "h0" ] ],
    [ "btn3:1.r", "bb1:bp.39", "green", [ "v0" ] ],
    [ "r2:1", "btn4:2.r", "green", [ "h0", "v-9.6" ] ],
    [ "r2:2", "bb1:bn.46", "green", [ "h0" ] ],
    [ "btn4:1.r", "bb1:bp.48", "green", [ "v0" ] ],
    [ "uno:5V", "bb1:bn.1", "red", [ "v-49.5", "h-293.8", "v519.7" ] ],
    [
      "uno:13",
      "bb1:22b.f",
      "green",
      [ "v27.2", "h542.8", "v374.4", "h-556.8", "v-211.2", "h38.4" ]
    ],
    [
      "uno:12",
      "bb1:34b.f",
      "green",
      [ "v36.8", "h542.7", "v355.2", "h-422.4", "v-201.6", "h19.2" ]
    ],
    [
      "bb1:46b.f",
      "uno:11",
      "green",
      [ "v-19.2", "h-28.8", "v172.8", "h297.6", "v-316.8", "h-547.2" ]
    ],
    [
      "bb1:57b.f",
      "uno:10",
      "green",
      [ "v-19.2", "h-38.4", "v163.2", "h192", "v-297.6", "h-547.2" ]
    ],
    [ "bz1:2", "bb1:11t.a", "green", [ "h9.6", "v9.2" ] ],
    [ "btn2:1.l", "bb1:36b.g", "", [ "$bb" ] ],
    [ "btn2:2.l", "bb1:34b.g", "", [ "$bb" ] ],
    [ "btn2:1.r", "bb1:36b.j", "", [ "$bb" ] ],
    [ "btn2:2.r", "bb1:34b.j", "", [ "$bb" ] ],
    [ "btn1:1.l", "bb1:24b.g", "", [ "$bb" ] ],
    [ "btn1:2.l", "bb1:22b.g", "", [ "$bb" ] ],
    [ "btn1:1.r", "bb1:24b.j", "", [ "$bb" ] ],
    [ "btn1:2.r", "bb1:22b.j", "", [ "$bb" ] ],
    [ "btn4:1.l", "bb1:59b.g", "", [ "$bb" ] ],
    [ "btn4:2.l", "bb1:57b.g", "", [ "$bb" ] ],
    [ "btn4:1.r", "bb1:59b.j", "", [ "$bb" ] ],
    [ "btn4:2.r", "bb1:57b.j", "", [ "$bb" ] ],
    [ "btn3:1.l", "bb1:48b.g", "", [ "$bb" ] ],
    [ "btn3:2.l", "bb1:46b.g", "", [ "$bb" ] ],
    [ "btn3:1.r", "bb1:48b.j", "", [ "$bb" ] ],
    [ "btn3:2.r", "bb1:46b.j", "", [ "$bb" ] ],
    [ "bb1:11t.b", "uno:7", "green", [ "h67.2", "v-152" ] ],
    [ "bz1:1", "bb1:tn.6", "", [ "$bb" ] ],
    [ "r6:1", "bb1:24t.b", "", [ "$bb" ] ],
    [ "r6:2", "bb1:30t.b", "", [ "$bb" ] ],
    [ "led1:C", "bb1:tn.18", "", [ "$bb" ] ],
    [ "uno:2", "bb1:30t.a", "black", [ "v27.2", "h20.7" ] ],
    [ "led1:A", "bb1:24t.a", "green", [ "h0" ] ],
    [ "led3:C", "bb1:tn.28", "", [ "$bb" ] ],
    [ "led3:A", "bb1:36t.a", "green", [ "h0" ] ],
    [ "r8:1", "bb1:36t.b", "", [ "$bb" ] ],
    [ "r8:2", "bb1:42t.b", "", [ "$bb" ] ],
    [ "bb1:42t.a", "uno:3", "black", [ "v-105.6", "h-308.8" ] ],
    [ "led4:C", "bb1:tn.38", "", [ "$bb" ] ],
    [ "led4:A", "bb1:48t.a", "green", [ "h0" ] ],
    [ "r5:1", "bb1:48t.b", "", [ "$bb" ] ],
    [ "r5:2", "bb1:54t.b", "", [ "$bb" ] ],
    [ "bb1:54t.a", "uno:4", "black", [ "v-96", "h-414.5" ] ],
    [ "led2:C", "bb1:tn.46", "", [ "$bb" ] ],
    [ "r7:1", "bb1:59t.b", "", [ "$bb" ] ],
    [ "led2:A", "bb1:59t.a", "green", [ "h0" ] ],
    [ "r7:2", "uno:5", "black", [ "v-86.4", "h-511.8" ] ],
    [ "uno:GND.3", "bb1:tn.1", "black", [ "v-30.3", "h-36.8" ] ],
    [ "bb1:tn.2", "bb1:bp.2", "green", [ "v0" ] ]
  ],
  "dependencies": {}
}
