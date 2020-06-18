# REACT 练习代码

import React from "react";
import ReactDom from "react-dom";

function myFun() {
  window.alert("hello world");
}

const myFun1 = () => {
  window.alert("how are you");
};

const e = React.createElement("input", {
  id: "input",
  type: "number",
  style: {
    color: "red",
    border: "2px solid green",
    borderRadius: "4px"
  },
  onInput: myFun1
});

const liOne = React.createElement("li", {}, "12121212123");
const liTwo = React.createElement("li", {}, "343434343434");
const e2 = React.createElement("ul", {}, [liOne, liTwo]);
const e3 = (
  <ul>
    <li>123</li>
    <li>43545</li>
  </ul>
);

const btn = <button />;

const ipt = React.createElement("input", {
  className: "inout",
  type: "number",
  style: {
    backgroundColor: "red",
    color: "blue"
  },
  onInput: () => {
    window.alert("shgdhkasdhkjsadkj");
  }
});

const ipt1 = (
  <input
    className={"input"}
    type={"number"}
    style={{ backgroundColor: "red", color: "green" }}
    onInput={() => {
      window.alert("wyque764832648ewu");
    }}
  />
);

const ew1 = (
  <div>
    <ul>
      <li>168723687</li>
      <li>1238768732864738674</li>
    </ul>
  </div>
);

const rootE = document.getElementById("root");
ReactDom.render(e, rootE);
ReactDom.render(e2, rootE);
ReactDom.render(ew1, rootE);
