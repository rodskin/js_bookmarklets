function getParameterByName(name, url) {
    if (!url) url = window.location.href;
    name = name.replace(/[\[\]]/g, '\\$&');
    var regex = new RegExp('[?&]' + name + '(=([^&#]*)|&|#|$)'), results = regex.exec(url);
    if (!results) return null;
    if (!results[2]) return '';
    return decodeURIComponent(results[2].replace(/\+/g, ' '));
}

nid_from_link = getParameterByName('node', document.querySelector('link[rel="delete-multiple-form"]').href)
var url = location.protocol+'//'+location.hostname+(location.port ? ':'+location.port: '');
nid = prompt("Enter nid", nid_from_link );
if (nid !== null) {
  window.location.href = url +"/node/"+ nid +"/edit";
}
