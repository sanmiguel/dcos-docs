---
post_title: Master Routes
menu_order: 1
---

Admin Router runs on DC/OS master nodes and exposes the following API routes, grouped by the component to which they proxy or relate.

<style>
#html-include code {
	padding: 0;
	padding-top: 0.2em;
	padding-bottom: 0.2em;
	margin: 0;
	font-size: 85%;
	font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier, monospace;
	background-color: inherit;
	color: inherit;
	border: 0;
}

#html-include .route-table {
	list-style-type: none;
	margin: 0;
	padding: 0;
}
#html-include .route {
	display: inline-block;
	width: calc(100% - 2px); /* subtract 2x border-width */
	margin: 0;
	/*padding: 0.5rem 1rem;*/
	line-height: 125%;
	border: 1px solid #000;
	border-radius: 3px;
	font-weight: 600;
	font-size: 1rem;
}
#html-include .route-type {
	display: inline-block;
	padding: 0.5rem;
	width: 5rem;
	text-align: center;
	text-transform: uppercase;
	text-decoration: none;
	font-weight: 300;
	font-size: 85%;
	color: #fff;
	border-radius: 3px;
}

#html-include .route-type-backend {
	background-color: rgba(16, 165, 74, 0.1);
	border-radius: 3px;
}
#html-include .route-type-redirect {
	background-color: rgba(197, 134, 43, 0.1);
	border-radius: 3px;
}
#html-include .route-type-file {
	background-color: rgba(15, 106, 180, 0.1);
	border-radius: 3px;
}
#html-include .route-type-unknown {
	background-color: rgba(66, 66, 66, 0.1);
	border-radius: 3px;
}

#html-include .route-type-backend .route {
	border-color: rgba(16, 165, 74, 0.3);
}
#html-include .route-type-redirect .route {
	border-color: rgba(197, 134, 43, 0.3);
}
#html-include .route-type-file .route {
	border-color: rgba(15, 106, 180, 0.3);
}
#html-include .route-type-unknown .route {
	border-color: rgba(66, 66, 66, 0.3);
}

#html-include .route-type-backend .route-type {
	background-color: rgba(16, 165, 74, 1.0);
}
#html-include .route-type-redirect .route-type {
	background-color: rgba(197, 134, 43, 1.0);
}
#html-include .route-type-file .route-type {
	background-color: rgba(15, 106, 180, 1.0);
}
#html-include .route-type-unknown .route-type {
	background-color: rgba(66, 66, 66, 1.0);
}

#html-include .route-type-backend .route-desc {
	color: rgba(16, 165, 74, 1.0);
}
#html-include .route-type-redirect .route-desc {
	color: rgba(197, 134, 43, 1.0);
}
#html-include .route-type-file .route-desc {
	color: rgba(15, 106, 180, 1.0);
}
#html-include .route-type-unknown .route-desc {
	color: rgba(66, 66, 66, 1.0);
}

#html-include .route-path {
	display: inline-block;
	padding: 0.5rem;
	vertical-align: middle;
}
#html-include .route-desc {
	right: 0;
	display: block;
	float: right;
	padding: 0.5rem 1rem;
	font-weight: 400;
	vertical-align: middle;
}
#html-include .route-meta {
	padding: 0.5rem;
	border: 1px solid #c3e8d1;
	border-top: 0;
	border-radius: 3px;
}
#html-include .route-meta table {
	width: 100%;
	border: 1px solid rgba(0,0,0,0.1);
	border-collapse: collapse;
	border-spacing: 0;
}
#html-include .route-meta table tr:nth-child(even) {
	background-color: rgba(0,0,0,0.05);
}
#html-include .route-meta table tr td {
	padding: 1rem;
	line-height: 125%;
}
#html-include .route-meta table tr td:first-child {
	width: 4rem;
}
</style>

<div id="html-include" class="html-include" data-api="/docs/1.9/api/nginx.master.html">
	<div class="info" id="api_info">
		<div class="info_title">Loading docs...</div>
	<div class="info_description markdown"></div>
</div>

<script>
(function() {
	var parent = document.getElementById("html-include");
	var file = parent.getAttribute("data-api");
	if (file) {
		var xhttp = new XMLHttpRequest();
		xhttp.onreadystatechange = function() {
			if (this.readyState == 4 && this.status == 200) {
				parent.innerHTML = this.responseText;
				parent.removeAttribute("data-api");
			}
		};
		xhttp.open("GET", file, true);
		xhttp.send();
	}
}());
<script>
