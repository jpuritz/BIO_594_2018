<!DOCTYPE html>
<html>
  <head>
      <meta charset="utf-8" />
      <title>finalproject</title>
      <style>.markdown-preview:not([data-use-github-style]) { padding: 2em; font-size: 1.2em; color: rgb(246, 248, 250); background-color: rgb(36, 41, 46); overflow: auto; }
.markdown-preview:not([data-use-github-style]) > :first-child { margin-top: 0px; }
.markdown-preview:not([data-use-github-style]) h1, .markdown-preview:not([data-use-github-style]) h2, .markdown-preview:not([data-use-github-style]) h3, .markdown-preview:not([data-use-github-style]) h4, .markdown-preview:not([data-use-github-style]) h5, .markdown-preview:not([data-use-github-style]) h6 { line-height: 1.2; margin-top: 1.5em; margin-bottom: 0.5em; color: rgb(255, 255, 255); }
.markdown-preview:not([data-use-github-style]) h1 { font-size: 2.4em; font-weight: 300; }
.markdown-preview:not([data-use-github-style]) h2 { font-size: 1.8em; font-weight: 400; }
.markdown-preview:not([data-use-github-style]) h3 { font-size: 1.5em; font-weight: 500; }
.markdown-preview:not([data-use-github-style]) h4 { font-size: 1.2em; font-weight: 600; }
.markdown-preview:not([data-use-github-style]) h5 { font-size: 1.1em; font-weight: 600; }
.markdown-preview:not([data-use-github-style]) h6 { font-size: 1em; font-weight: 600; }
.markdown-preview:not([data-use-github-style]) strong { color: rgb(255, 255, 255); }
.markdown-preview:not([data-use-github-style]) del { color: rgb(194, 207, 221); }
.markdown-preview:not([data-use-github-style]) a, .markdown-preview:not([data-use-github-style]) a code { color: rgb(255, 255, 255); }
.markdown-preview:not([data-use-github-style]) img { max-width: 100%; }
.markdown-preview:not([data-use-github-style]) > p { margin-top: 0px; margin-bottom: 1.5em; }
.markdown-preview:not([data-use-github-style]) > ul, .markdown-preview:not([data-use-github-style]) > ol { margin-bottom: 1.5em; }
.markdown-preview:not([data-use-github-style]) blockquote { margin: 1.5em 0px; font-size: inherit; color: rgb(194, 207, 221); border-color: rgb(72, 82, 92); border-width: 4px; }
.markdown-preview:not([data-use-github-style]) hr { margin: 3em 0px; border-top: 2px dashed rgb(72, 82, 92); background: none; }
.markdown-preview:not([data-use-github-style]) table { margin: 1.5em 0px; }
.markdown-preview:not([data-use-github-style]) th { color: rgb(255, 255, 255); }
.markdown-preview:not([data-use-github-style]) th, .markdown-preview:not([data-use-github-style]) td { padding: 0.66em 1em; border: 1px solid rgb(72, 82, 92); }
.markdown-preview:not([data-use-github-style]) code { color: rgb(255, 255, 255); background-color: rgb(54, 61, 69); }
.markdown-preview:not([data-use-github-style]) pre.editor-colors { margin: 1.5em 0px; padding: 1em; font-size: 0.92em; border-radius: 3px; background-color: rgb(45, 51, 57); }
.markdown-preview:not([data-use-github-style]) kbd { color: rgb(255, 255, 255); border-width: 1px 1px 2px; border-style: solid; border-color: rgb(72, 82, 92) rgb(72, 82, 92) rgb(58, 66, 75); border-image: initial; background-color: rgb(54, 61, 69); }
.markdown-preview[data-use-github-style] { font-family: "Helvetica Neue", Helvetica, "Segoe UI", Arial, freesans, sans-serif; line-height: 1.6; word-wrap: break-word; padding: 30px; font-size: 16px; color: rgb(51, 51, 51); background-color: rgb(255, 255, 255); overflow: scroll; }
.markdown-preview[data-use-github-style] > :first-child { margin-top: 0px !important; }
.markdown-preview[data-use-github-style] > :last-child { margin-bottom: 0px !important; }
.markdown-preview[data-use-github-style] a:not([href]) { color: inherit; text-decoration: none; }
.markdown-preview[data-use-github-style] .absent { color: rgb(204, 0, 0); }
.markdown-preview[data-use-github-style] .anchor { position: absolute; top: 0px; left: 0px; display: block; padding-right: 6px; padding-left: 30px; margin-left: -30px; }
.markdown-preview[data-use-github-style] .anchor:focus { outline: none; }
.markdown-preview[data-use-github-style] h1, .markdown-preview[data-use-github-style] h2, .markdown-preview[data-use-github-style] h3, .markdown-preview[data-use-github-style] h4, .markdown-preview[data-use-github-style] h5, .markdown-preview[data-use-github-style] h6 { position: relative; margin-top: 1em; margin-bottom: 16px; font-weight: bold; line-height: 1.4; }
.markdown-preview[data-use-github-style] h1 .octicon-link, .markdown-preview[data-use-github-style] h2 .octicon-link, .markdown-preview[data-use-github-style] h3 .octicon-link, .markdown-preview[data-use-github-style] h4 .octicon-link, .markdown-preview[data-use-github-style] h5 .octicon-link, .markdown-preview[data-use-github-style] h6 .octicon-link { display: none; color: rgb(0, 0, 0); vertical-align: middle; }
.markdown-preview[data-use-github-style] h1:hover .anchor, .markdown-preview[data-use-github-style] h2:hover .anchor, .markdown-preview[data-use-github-style] h3:hover .anchor, .markdown-preview[data-use-github-style] h4:hover .anchor, .markdown-preview[data-use-github-style] h5:hover .anchor, .markdown-preview[data-use-github-style] h6:hover .anchor { padding-left: 8px; margin-left: -30px; text-decoration: none; }
.markdown-preview[data-use-github-style] h1:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h2:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h3:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h4:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h5:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h6:hover .anchor .octicon-link { display: inline-block; }
.markdown-preview[data-use-github-style] h1 tt, .markdown-preview[data-use-github-style] h2 tt, .markdown-preview[data-use-github-style] h3 tt, .markdown-preview[data-use-github-style] h4 tt, .markdown-preview[data-use-github-style] h5 tt, .markdown-preview[data-use-github-style] h6 tt, .markdown-preview[data-use-github-style] h1 code, .markdown-preview[data-use-github-style] h2 code, .markdown-preview[data-use-github-style] h3 code, .markdown-preview[data-use-github-style] h4 code, .markdown-preview[data-use-github-style] h5 code, .markdown-preview[data-use-github-style] h6 code { font-size: inherit; }
.markdown-preview[data-use-github-style] h1 { padding-bottom: 0.3em; font-size: 2.25em; line-height: 1.2; border-bottom: 1px solid rgb(238, 238, 238); }
.markdown-preview[data-use-github-style] h1 .anchor { line-height: 1; }
.markdown-preview[data-use-github-style] h2 { padding-bottom: 0.3em; font-size: 1.75em; line-height: 1.225; border-bottom: 1px solid rgb(238, 238, 238); }
.markdown-preview[data-use-github-style] h2 .anchor { line-height: 1; }
.markdown-preview[data-use-github-style] h3 { font-size: 1.5em; line-height: 1.43; }
.markdown-preview[data-use-github-style] h3 .anchor { line-height: 1.2; }
.markdown-preview[data-use-github-style] h4 { font-size: 1.25em; }
.markdown-preview[data-use-github-style] h4 .anchor { line-height: 1.2; }
.markdown-preview[data-use-github-style] h5 { font-size: 1em; }
.markdown-preview[data-use-github-style] h5 .anchor { line-height: 1.1; }
.markdown-preview[data-use-github-style] h6 { font-size: 1em; color: rgb(119, 119, 119); }
.markdown-preview[data-use-github-style] h6 .anchor { line-height: 1.1; }
.markdown-preview[data-use-github-style] p, .markdown-preview[data-use-github-style] blockquote, .markdown-preview[data-use-github-style] ul, .markdown-preview[data-use-github-style] ol, .markdown-preview[data-use-github-style] dl, .markdown-preview[data-use-github-style] table, .markdown-preview[data-use-github-style] pre { margin-top: 0px; margin-bottom: 16px; }
.markdown-preview[data-use-github-style] hr { height: 4px; padding: 0px; margin: 16px 0px; background-color: rgb(231, 231, 231); border: 0px none; }
.markdown-preview[data-use-github-style] ul, .markdown-preview[data-use-github-style] ol { padding-left: 2em; }
.markdown-preview[data-use-github-style] ul.no-list, .markdown-preview[data-use-github-style] ol.no-list { padding: 0px; list-style-type: none; }
.markdown-preview[data-use-github-style] ul ul, .markdown-preview[data-use-github-style] ul ol, .markdown-preview[data-use-github-style] ol ol, .markdown-preview[data-use-github-style] ol ul { margin-top: 0px; margin-bottom: 0px; }
.markdown-preview[data-use-github-style] li > p { margin-top: 16px; }
.markdown-preview[data-use-github-style] dl { padding: 0px; }
.markdown-preview[data-use-github-style] dl dt { padding: 0px; margin-top: 16px; font-size: 1em; font-style: italic; font-weight: bold; }
.markdown-preview[data-use-github-style] dl dd { padding: 0px 16px; margin-bottom: 16px; }
.markdown-preview[data-use-github-style] blockquote { padding: 0px 15px; color: rgb(119, 119, 119); border-left: 4px solid rgb(221, 221, 221); }
.markdown-preview[data-use-github-style] blockquote > :first-child { margin-top: 0px; }
.markdown-preview[data-use-github-style] blockquote > :last-child { margin-bottom: 0px; }
.markdown-preview[data-use-github-style] table { display: block; width: 100%; overflow: auto; word-break: keep-all; }
.markdown-preview[data-use-github-style] table th { font-weight: bold; }
.markdown-preview[data-use-github-style] table th, .markdown-preview[data-use-github-style] table td { padding: 6px 13px; border: 1px solid rgb(221, 221, 221); }
.markdown-preview[data-use-github-style] table tr { background-color: rgb(255, 255, 255); border-top: 1px solid rgb(204, 204, 204); }
.markdown-preview[data-use-github-style] table tr:nth-child(2n) { background-color: rgb(248, 248, 248); }
.markdown-preview[data-use-github-style] img { max-width: 100%; box-sizing: border-box; }
.markdown-preview[data-use-github-style] .emoji { max-width: none; }
.markdown-preview[data-use-github-style] span.frame { display: block; overflow: hidden; }
.markdown-preview[data-use-github-style] span.frame > span { display: block; float: left; width: auto; padding: 7px; margin: 13px 0px 0px; overflow: hidden; border: 1px solid rgb(221, 221, 221); }
.markdown-preview[data-use-github-style] span.frame span img { display: block; float: left; }
.markdown-preview[data-use-github-style] span.frame span span { display: block; padding: 5px 0px 0px; clear: both; color: rgb(51, 51, 51); }
.markdown-preview[data-use-github-style] span.align-center { display: block; overflow: hidden; clear: both; }
.markdown-preview[data-use-github-style] span.align-center > span { display: block; margin: 13px auto 0px; overflow: hidden; text-align: center; }
.markdown-preview[data-use-github-style] span.align-center span img { margin: 0px auto; text-align: center; }
.markdown-preview[data-use-github-style] span.align-right { display: block; overflow: hidden; clear: both; }
.markdown-preview[data-use-github-style] span.align-right > span { display: block; margin: 13px 0px 0px; overflow: hidden; text-align: right; }
.markdown-preview[data-use-github-style] span.align-right span img { margin: 0px; text-align: right; }
.markdown-preview[data-use-github-style] span.float-left { display: block; float: left; margin-right: 13px; overflow: hidden; }
.markdown-preview[data-use-github-style] span.float-left span { margin: 13px 0px 0px; }
.markdown-preview[data-use-github-style] span.float-right { display: block; float: right; margin-left: 13px; overflow: hidden; }
.markdown-preview[data-use-github-style] span.float-right > span { display: block; margin: 13px auto 0px; overflow: hidden; text-align: right; }
.markdown-preview[data-use-github-style] code, .markdown-preview[data-use-github-style] tt { padding: 0.2em 0px; margin: 0px; font-size: 85%; background-color: rgba(0, 0, 0, 0.04); border-radius: 3px; }
.markdown-preview[data-use-github-style] code::before, .markdown-preview[data-use-github-style] tt::before, .markdown-preview[data-use-github-style] code::after, .markdown-preview[data-use-github-style] tt::after { letter-spacing: -0.2em; content: " "; }
.markdown-preview[data-use-github-style] code br, .markdown-preview[data-use-github-style] tt br { display: none; }
.markdown-preview[data-use-github-style] del code { text-decoration: inherit; }
.markdown-preview[data-use-github-style] pre > code { padding: 0px; margin: 0px; font-size: 100%; word-break: normal; white-space: pre; background: transparent; border: 0px; }
.markdown-preview[data-use-github-style] .highlight { margin-bottom: 16px; }
.markdown-preview[data-use-github-style] .highlight pre, .markdown-preview[data-use-github-style] pre { padding: 16px; overflow: auto; font-size: 85%; line-height: 1.45; background-color: rgb(247, 247, 247); border-radius: 3px; }
.markdown-preview[data-use-github-style] .highlight pre { margin-bottom: 0px; word-break: normal; }
.markdown-preview[data-use-github-style] pre { word-wrap: normal; }
.markdown-preview[data-use-github-style] pre code, .markdown-preview[data-use-github-style] pre tt { display: inline; max-width: initial; padding: 0px; margin: 0px; overflow: initial; line-height: inherit; word-wrap: normal; background-color: transparent; border: 0px; }
.markdown-preview[data-use-github-style] pre code::before, .markdown-preview[data-use-github-style] pre tt::before, .markdown-preview[data-use-github-style] pre code::after, .markdown-preview[data-use-github-style] pre tt::after { content: normal; }
.markdown-preview[data-use-github-style] kbd { display: inline-block; padding: 3px 5px; font-size: 11px; line-height: 10px; color: rgb(85, 85, 85); vertical-align: middle; background-color: rgb(252, 252, 252); border-width: 1px; border-style: solid; border-color: rgb(204, 204, 204) rgb(204, 204, 204) rgb(187, 187, 187); border-image: initial; border-radius: 3px; box-shadow: rgb(187, 187, 187) 0px -1px 0px inset; }
.markdown-preview[data-use-github-style] a { color: rgb(51, 122, 183); }
.markdown-preview[data-use-github-style] code { color: inherit; }
.markdown-preview[data-use-github-style] pre.editor-colors { padding: 0.8em 1em; margin-bottom: 1em; font-size: 0.85em; border-radius: 4px; overflow: auto; }
.scrollbars-visible-always .markdown-preview pre.editor-colors .vertical-scrollbar, .scrollbars-visible-always .markdown-preview pre.editor-colors .horizontal-scrollbar { visibility: hidden; }
.scrollbars-visible-always .markdown-preview pre.editor-colors:hover .vertical-scrollbar, .scrollbars-visible-always .markdown-preview pre.editor-colors:hover .horizontal-scrollbar { visibility: visible; }
.markdown-preview .task-list-item-checkbox { position: absolute; margin: 0.25em 0px 0px -1.4em; }
.bracket-matcher .region {
  border-bottom: 1px dotted lime;
  position: absolute;
}
.line-number.bracket-matcher.bracket-matcher {
  color: #f6f8fa;
  background-color: #444d56;
}

.spell-check-misspelling .region {
  border-bottom: 2px dotted rgba(255, 51, 51, 0.75);
}
.spell-check-corrections {
  width: 25em !important;
}

pre.editor-colors {
  background-color: #24292e;
  color: #f6f8fa;
}
pre.editor-colors .line.cursor-line {
  background-color: #444d56;
}
pre.editor-colors .invisible {
  color: #6a737d;
}
pre.editor-colors .cursor {
  border-left: 2px solid #fff;
}
pre.editor-colors .selection .region {
  background-color: #4c2889;
}
pre.editor-colors .bracket-matcher .region {
  border-bottom: 1px solid #fff;
  box-sizing: border-box;
  z-index: 1;
}
pre.editor-colors .invisible-character {
  color: #6a737d;
}
pre.editor-colors .indent-guide {
  color: #6a737d;
}
pre.editor-colors .wrap-guide {
  background-color: #6a737d;
}
pre.editor-colors .gutter {
  background-color: #24292e;
  color: #f6f8fa;
}
pre.editor-colors .gutter .line-number {
  color: #f6f8fa;
  -webkit-font-smoothing: antialiased;
}
pre.editor-colors .gutter .line-number.cursor-line {
  color: #f6f8fa;
  background-color: #444d56;
}
pre.editor-colors .gutter .line-number.cursor-line-no-selection {
  background-color: transparent;
}
pre.editor-colors .gutter .line-number .icon-right {
  color: #f6f8fa;
}
pre.editor-colors .gutter:not(.git-diff-icon) .line-number.git-line-removed.git-line-removed::before {
  bottom: -3px;
}
pre.editor-colors .gutter:not(.git-diff-icon) .line-number.git-line-removed::after {
  content: "";
  position: absolute;
  left: 0px;
  bottom: 0px;
  width: 25px;
  border-bottom: 1px dotted rgba(215, 58, 73, 0.5);
  pointer-events: none;
}
pre.editor-colors .gutter .line-number.folded,
pre.editor-colors .gutter .line-number:after,
pre.editor-colors .fold-marker:after {
  color: #f6f8fa;
}
pre.editor-colors .search-results .syntax--marker .region {
  background-color: transparent;
  border: 1px solid #fb8532;
}
pre.editor-colors .search-results .syntax--marker.current-result .region {
  border: 1px solid #24292e;
}
pre.editor-colors .syntax--comment,
pre.editor-colors .syntax--punctuation.syntax--definition.syntax--comment,
pre.editor-colors .syntax--string.syntax--comment {
  color: #959da5;
}
pre.editor-colors .syntax--constant,
pre.editor-colors .syntax--entity.syntax--name.syntax--constant,
pre.editor-colors .syntax--variable.syntax--other.syntax--constant,
pre.editor-colors .syntax--variable.syntax--language {
  color: #c8e1ff;
}
pre.editor-colors .syntax--entity,
pre.editor-colors .syntax--entity.syntax--name {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #b392f0;
}
pre.editor-colors .syntax--variable.syntax--parameter.syntax--function {
  color: #f6f8fa;
}
pre.editor-colors .syntax--entity.syntax--name.syntax--tag {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #7bcc72;
}
pre.editor-colors .syntax--keyword {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #ea4a5a;
}
pre.editor-colors .syntax--storage,
pre.editor-colors .syntax--storage.syntax--type {
  color: #ea4a5a;
}
pre.editor-colors .syntax--storage.syntax--modifier.syntax--package,
pre.editor-colors .syntax--storage.syntax--modifier.syntax--import,
pre.editor-colors .syntax--storage.syntax--type.syntax--java {
  color: #f6f8fa;
}
pre.editor-colors .syntax--string,
pre.editor-colors .syntax--punctuation.syntax--definition.syntax--string,
pre.editor-colors .syntax--string .syntax--punctuation.syntax--section.syntax--embedded .syntax--source {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #79b8ff;
}
pre.editor-colors .syntax--support {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #c8e1ff;
}
pre.editor-colors .syntax--meta.syntax--property-name {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #c8e1ff;
}
pre.editor-colors .syntax--variable {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #fb8532;
}
pre.editor-colors .syntax--variable.syntax--other {
  color: #f6f8fa;
}
pre.editor-colors .syntax--invalid.syntax--broken {
  font-weight: bold;
  font-style: italic;
  text-decoration: underline;
  color: #d73a49;
}
pre.editor-colors .syntax--invalid.syntax--deprecated {
  font-weight: bold;
  font-style: italic;
  text-decoration: underline;
  color: #d73a49;
}
pre.editor-colors .syntax--invalid.syntax--illegal {
  font-style: italic;
  text-decoration: underline;
  color: #fafbfc;
  background-color: #d73a49;
}
pre.editor-colors .syntax--carriage-return {
  font-style: italic;
  text-decoration: underline;
  color: #fafbfc;
  background-color: #d73a49;
  undefined: ^M;
}
pre.editor-colors .syntax--invalid.syntax--unimplemented {
  font-weight: bold;
  font-style: italic;
  text-decoration: underline;
  color: #d73a49;
}
pre.editor-colors .syntax--message.syntax--error {
  color: #d73a49;
}
pre.editor-colors .syntax--string .syntax--source {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #f6f8fa;
}
pre.editor-colors .syntax--string .syntax--variable {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #c8e1ff;
}
pre.editor-colors .syntax--source.syntax--regexp,
pre.editor-colors .syntax--string.syntax--regexp {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #79b8ff;
}
pre.editor-colors .syntax--string.syntax--regexp.syntax--character-class,
pre.editor-colors .syntax--string.syntax--regexp .syntax--constant.syntax--character.syntax--escape,
pre.editor-colors .syntax--string.syntax--regexp .syntax--source.syntax--ruby.syntax--embedded,
pre.editor-colors .syntax--string.syntax--regexp .syntax--string.syntax--regexp.syntax--arbitrary-repitition {
  color: #79b8ff;
}
pre.editor-colors .syntax--string.syntax--regexp .syntax--constant.syntax--character.syntax--escape {
  font-weight: bold;
  color: #7bcc72;
}
pre.editor-colors .syntax--support.syntax--constant {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #c8e1ff;
}
pre.editor-colors .syntax--support.syntax--variable {
  color: #c8e1ff;
}
pre.editor-colors .syntax--meta.syntax--module-reference {
  color: #c8e1ff;
}
pre.editor-colors .syntax--markup.syntax--list {
  color: #fb8532;
}
pre.editor-colors .syntax--markup.syntax--heading,
pre.editor-colors .syntax--markup.syntax--heading .syntax--entity.syntax--name {
  font-weight: bold;
  color: #0366d6;
}
pre.editor-colors .syntax--markup.syntax--quote {
  color: #c8e1ff;
}
pre.editor-colors .syntax--markup.syntax--italic {
  font-style: italic;
  color: #f6f8fa;
}
pre.editor-colors .syntax--markup.syntax--bold {
  font-weight: bold;
  color: #f6f8fa;
}
pre.editor-colors .syntax--markup.syntax--raw {
  font-weight: normal;
  font-style: normal;
  text-decoration: none;
  color: #c8e1ff;
}
pre.editor-colors .syntax--markup.syntax--deleted,
pre.editor-colors .syntax--meta.syntax--diff.syntax--header.syntax--from-file,
pre.editor-colors .syntax--punctuation.syntax--definition.syntax--deleted {
  background-color: #ffeef0;
  color: #b31d28;
}
pre.editor-colors .syntax--markup.syntax--inserted,
pre.editor-colors .syntax--meta.syntax--diff.syntax--header.syntax--to-file,
pre.editor-colors .syntax--punctuation.syntax--definition.syntax--inserted {
  background-color: #f0fff4;
  color: #176f2c;
}
pre.editor-colors .syntax--markup.syntax--changed,
pre.editor-colors .syntax--punctuation.syntax--definition.syntax--changed {
  background-color: #fffdef;
  color: #b08800;
}
pre.editor-colors .syntax--markup.syntax--ignored,
pre.editor-colors .syntax--markup.syntax--untracked {
  color: #2f363d;
  background-color: #959da5;
}
pre.editor-colors .syntax--meta.syntax--diff.syntax--range {
  font-weight: bold;
  color: #b392f0;
}
pre.editor-colors .syntax--meta.syntax--diff.syntax--header {
  color: #c8e1ff;
}
pre.editor-colors .syntax--meta.syntax--separator {
  font-weight: bold;
  color: #0366d6;
}
pre.editor-colors .syntax--meta.syntax--output {
  color: #0366d6;
}
pre.editor-colors .syntax--brackethighlighter.syntax--tag,
pre.editor-colors .syntax--brackethighlighter.syntax--curly,
pre.editor-colors .syntax--brackethighlighter.syntax--round,
pre.editor-colors .syntax--brackethighlighter.syntax--square,
pre.editor-colors .syntax--brackethighlighter.syntax--angle,
pre.editor-colors .syntax--brackethighlighter.syntax--quote {
  color: #ffeef0;
}
pre.editor-colors .syntax--brackethighlighter.syntax--unmatched {
  color: #d73a49;
}
pre.editor-colors .syntax--sublimelinter.syntax--mark.syntax--error {
  color: #d73a49;
}
pre.editor-colors .syntax--sublimelinter.syntax--mark.syntax--warning {
  color: #fb8532;
}
pre.editor-colors .syntax--sublimelinter.syntax--gutter-mark {
  color: #6a737d;
}
pre.editor-colors .syntax--constant.syntax--other.syntax--reference.syntax--link,
pre.editor-colors .syntax--string.syntax--other.syntax--link {
  color: #79b8ff;
  text-decoration: underline;
}
</style>
  </head>
  <body class='markdown-preview' data-use-github-style><h1 id="-trimming-assembly-sorting-"><strong>Trimming, Assembly, Sorting</strong></h1>
<h2 id="fastqc-quality-check">FastQC Quality Check</h2>
<pre class="editor-colors lang-#!/bin/bash"><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#SBATCH&nbsp;-J&nbsp;Neph</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#SBATCH&nbsp;-t&nbsp;4-00:00:00</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#SBATCH&nbsp;-N&nbsp;1</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#SBATCH&nbsp;-n&nbsp;16</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>module&nbsp;load&nbsp;FastQC/0.11.5-Java-1.8.0_92</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>fastqc&nbsp;*.gz</span></span></div></pre>
<h2 id="trimmomatic">Trimmomatic</h2>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shebang syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shebang syntax--shell"><span>#!</span></span><span>/bin/bash</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-J&nbsp;Nephtrim</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-t&nbsp;4-00:00:00</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-N&nbsp;1</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-n&nbsp;16</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>module&nbsp;load&nbsp;Trimmomatic/0.36-Java-1.8.0_92</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>java&nbsp;-jar&nbsp;</span><span class="syntax--variable syntax--other syntax--normal syntax--shell"><span class="syntax--punctuation syntax--definition syntax--variable syntax--shell"><span>$</span></span><span>EBROOTTRIMMOMATIC</span></span><span>/trimmomatic-0.36.jar&nbsp;PE&nbsp;-threads&nbsp;8&nbsp;-phred33&nbsp;XRICL_20160311_K00134_IL100067075_S24_L005_R1.fastq.gz&nbsp;XRICL_20160311_K00134_IL100067075_S24_L005_R2.fastq.gz&nbsp;nephPR1.fq.gz&nbsp;nephUPR1.fq.gz&nbsp;nephPR2.fq.gz&nbsp;nephUPR2.fq.gz&nbsp;ILLUMINACLIP:TruSeq3-PE.fa:2:30:10&nbsp;HEADCROP:&nbsp;13&nbsp;LEADING:4&nbsp;TRAILING:4&nbsp;SLIDINGWINDOW:4:20&nbsp;MINLEN:25</span></span></div></pre><pre class="editor-colors lang-"><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>TrimmomaticPE:&nbsp;Started&nbsp;with&nbsp;arguments:</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;-threads&nbsp;8&nbsp;-phred33&nbsp;XRICL_20160311_K00134_IL100067075_S24_L005_R1.fastq.gz&nbsp;XRICL_20160311_K00134_IL100067075_S24_L005_R2.fastq.gz&nbsp;nephPR1.fq.gz&nbsp;nephUPR1.fq.gz&nbsp;nephPR2.fq.gz&nbsp;nephUPR2.fq.gz&nbsp;ILLUMINACLIP:TruSeq3-PE.fa:2:30:10&nbsp;HEADCROP:13&nbsp;LEADING:4&nbsp;TRAILING:4&nbsp;SLIDINGWINDOW:4:20&nbsp;MINLEN:25</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;Using&nbsp;PrefixPair:&nbsp;'TACACTCTTTCCCTACACGACGCTCTTCCGATCT'&nbsp;and&nbsp;'GTGACTGGAGTTCAGACGTGTGCTCTTCCGATCT'</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;ILLUMINACLIP:&nbsp;Using&nbsp;1&nbsp;prefix&nbsp;pairs,&nbsp;0&nbsp;forward/reverse&nbsp;sequences,&nbsp;0&nbsp;forward&nbsp;only&nbsp;sequences,&nbsp;0&nbsp;reverse&nbsp;only&nbsp;sequences</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;Input&nbsp;Read&nbsp;Pairs:&nbsp;55316212&nbsp;Both&nbsp;Surviving:&nbsp;39916756&nbsp;(72.16%)&nbsp;Forward&nbsp;Only&nbsp;Surviving:&nbsp;14602794&nbsp;(26.40%)&nbsp;Reverse&nbsp;Only&nbsp;Surviving:&nbsp;333261&nbsp;(0.60%)&nbsp;Dropped:&nbsp;463401&nbsp;(0.84%)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;TrimmomaticPE:&nbsp;Completed&nbsp;successfully</span></span></div></pre><p>*rechecked quality with FastQC</p>
<h2 id="trinity-assembly">Trinity Assembly</h2>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shebang syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shebang syntax--shell"><span>#!</span></span><span>/bin/bash</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-J&nbsp;CardioTrinity</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-t&nbsp;5-00:00:00</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;--mem=250G</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-N&nbsp;1</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;--exclusive</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;--mail-type=END</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;--mail-user=lizhunter@my.uri.edu</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>module&nbsp;load&nbsp;Trinity/2.4.0-foss-2016b</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>Bowtie2/2.2.9-foss-2016b</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>SAMtools/1.5-foss-2017a</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>Trinity&nbsp;\</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>--seqType&nbsp;fq&nbsp;\</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>--left&nbsp;cardioPR1.fq.gz&nbsp;\</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>--right&nbsp;cardioPR2.fq.gz&nbsp;\</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>--SS_lib_type&nbsp;FR&nbsp;\</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>--max_memory&nbsp;250G&nbsp;\</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>--CPU&nbsp;20&nbsp;\</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>--output&nbsp;</span><span class="syntax--keyword syntax--operator syntax--tilde syntax--shell"><span>~</span></span><span>/data3/lanelab/liz/BIO594/Cardio/Trinity</span></span></div></pre><h2 id="binning">Binning</h2>
<h3 id="prokaryotes-eukaryotes">Prokaryotes/Eukaryotes</h3>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#count&nbsp;sequences</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>grep&nbsp;"&gt;"&nbsp;$1&nbsp;|&nbsp;wc&nbsp;-l&nbsp;trinity.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#split&nbsp;into&nbsp;batches</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>awk&nbsp;'BEGIN&nbsp;{n_seq=0;}&nbsp;/^&gt;/&nbsp;{if(n_seq%100==0){file=sprintf("%d.fa",n_seq);}&nbsp;print&nbsp;&gt;&gt;&nbsp;file;&nbsp;n_seq++;&nbsp;next;}&nbsp;{&nbsp;print&nbsp;&gt;&gt;&nbsp;file;&nbsp;close(file)}'&nbsp;&lt;&nbsp;trinity.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#rename&nbsp;sequentially</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>n=1;&nbsp;for&nbsp;x&nbsp;in&nbsp;*.fa;&nbsp;do&nbsp;mv&nbsp;$x&nbsp;&nbsp;$n.fa;&nbsp;n=$(($n+1));&nbsp;done</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#run&nbsp;a&nbsp;blast&nbsp;array</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>blastx&nbsp;-query&nbsp;"SLURM_ARRAY_TASK_ID".fa&nbsp;-db&nbsp;refseq_protein&nbsp;-outfmt&nbsp;6&nbsp;-max_target_seqs&nbsp;1&nbsp;-max_hsps&nbsp;1&nbsp;-taxid&nbsp;-out&nbsp;"SLURM_ARRAY_TASK_ID".out</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>cat&nbsp;*.out&nbsp;nephall.txt</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#sort&nbsp;blast&nbsp;results&nbsp;by&nbsp;kingdom&nbsp;with&nbsp;regular&nbsp;expressions&nbsp;in&nbsp;text&nbsp;wrangler</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>grep&nbsp;"Prokaryotes"&nbsp;nephall.txt&nbsp;&gt;&nbsp;prokaryotes.txt</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>grep&nbsp;"Eukaryotes"&nbsp;nephall.txt&nbsp;&gt;&nbsp;eukaryotes.txt</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#Pull&nbsp;sequence&nbsp;IDs</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>(T.+\|m\.\d+)\t.+\n</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>Replace:&nbsp;\1\n</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#Pull&nbsp;Sequences&nbsp;Using&nbsp;Header&nbsp;File</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>grep&nbsp;-A1&nbsp;-w&nbsp;-f&nbsp;headers.txt&nbsp;trinity.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#generated&nbsp;a&nbsp;database&nbsp;of&nbsp;ascidians&nbsp;and&nbsp;apicomplexan&nbsp;transcriptomes</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>cat&nbsp;*.txt&nbsp;asciapi.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>makeblastdb&nbsp;-in&nbsp;asciapi.fasta&nbsp;-parse_seqids&nbsp;-dbtype&nbsp;nucl&nbsp;-taxid</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>blastx&nbsp;-query&nbsp;"SLURM_ARRAY_TASK_ID".fa&nbsp;-db&nbsp;asciapi.fasta&nbsp;-outfmt&nbsp;6&nbsp;-max_target_seqs&nbsp;1&nbsp;-max_hsps&nbsp;1&nbsp;-taxid&nbsp;-out&nbsp;"SLURM_ARRAY_TASK_ID".out</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>cat&nbsp;*.out&nbsp;&gt;&nbsp;asciapiblast.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#blast&nbsp;results&nbsp;sorted&nbsp;with&nbsp;regular&nbsp;expressions,&nbsp;sequence&nbsp;IDs&nbsp;sorted&nbsp;out,&nbsp;and&nbsp;the&nbsp;actually&nbsp;sequences&nbsp;pulled&nbsp;as&nbsp;above</span></span></div></pre><p>(in an ideal world with more time, would have remapped all raw reads to these bins with Bowtie then reassembled with trinity)</p>
<h2 id="translate-with-transdecoder">Translate with Transdecoder</h2>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>TransDecoder.LongOrfs&nbsp;-t&nbsp;nephtrinity.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>TransDecoder.Predict&nbsp;-t&nbsp;longest_orfs.cds</span></span></div></pre><h2 id="final-read-counts">Final Read Counts</h2>
<ul>
<li>Nephromyces 60,223</li>
<li>Cardiosporidium 15,541</li>
</ul>
<h1 id="-analysis-"><strong>Analysis</strong></h1>
<h2 id="busco-transcriptome-analysis">BUSCO Transcriptome Analysis</h2>
<h4 id="running-busco">Running BUSCO</h4>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shebang syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shebang syntax--shell"><span>#!</span></span><span>/bin/bash</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-J&nbsp;busco</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-t&nbsp;01:00:00</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-N&nbsp;1</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span class="syntax--comment syntax--line syntax--number-sign syntax--shell"><span class="syntax--punctuation syntax--definition syntax--comment syntax--shell"><span>#</span></span><span>SBATCH&nbsp;-n&nbsp;16</span></span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>module&nbsp;load&nbsp;busco/2.0</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>module&nbsp;load&nbsp;blast</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>module&nbsp;load&nbsp;HMMER/3.1b2-foss-2016b</span></span></div><div class="line"><span class="syntax--source syntax--shell"><span>python&nbsp;../run_BUSCO.py&nbsp;-i&nbsp;/data3/lanelab/liz/BIO594/Cardio/Trinity/cardiotrinity.fasta&nbsp;-o&nbsp;cardiobusco&nbsp;-l&nbsp;/data3/lanelab/liz/BIO594/alveolata_stramenophiles_ensembl&nbsp;-m&nbsp;tran</span></span></div></pre><h4 id="generation-of-r-code">Generation of R code</h4>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>conda&nbsp;create&nbsp;-n&nbsp;python36&nbsp;python=3.6&nbsp;anaconda</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>python&nbsp;BUSCO_plot.py&nbsp;-wd&nbsp;/Users/AlgaeLab/Desktop/LIZ/BUSCO/plot_data</span></span></div></pre><h4 id="busco-transcriptome-graphing-r-">Busco Transcriptome Graphing (R)</h4>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;BUSCO&nbsp;summary&nbsp;figure</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;@author&nbsp;Mathieu&nbsp;Seppey&nbsp;&lt;mathieu.seppey@unige.ch&gt;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;@version&nbsp;2.0</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;@since&nbsp;BUSCO&nbsp;2.0</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;Copyright&nbsp;(C)&nbsp;2016&nbsp;E.&nbsp;Zdobnov&nbsp;lab</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;BUSCO&nbsp;is&nbsp;free&nbsp;software:&nbsp;you&nbsp;can&nbsp;redistribute&nbsp;it&nbsp;and/or&nbsp;modify</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;it&nbsp;under&nbsp;the&nbsp;terms&nbsp;of&nbsp;the&nbsp;GNU&nbsp;General&nbsp;Public&nbsp;License&nbsp;as&nbsp;published&nbsp;by</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;the&nbsp;Free&nbsp;Software&nbsp;Foundation,&nbsp;either&nbsp;version&nbsp;3&nbsp;of&nbsp;the&nbsp;License,&nbsp;or</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;(at&nbsp;your&nbsp;option)&nbsp;any&nbsp;later&nbsp;version.&nbsp;See&nbsp;&lt;</span><span class="syntax--markup syntax--underline syntax--link syntax--http syntax--hyperlink"><span>http://www.gnu.org/licenses/</span></span><span>&gt;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;BUSCO&nbsp;is&nbsp;distributed&nbsp;in&nbsp;the&nbsp;hope&nbsp;that&nbsp;it&nbsp;will&nbsp;be&nbsp;useful,</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;but&nbsp;WITHOUT&nbsp;ANY&nbsp;WARRANTY;&nbsp;without&nbsp;even&nbsp;the&nbsp;implied&nbsp;warranty&nbsp;of</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;MERCHANTABILITY&nbsp;or&nbsp;FITNESS&nbsp;FOR&nbsp;A&nbsp;PARTICULAR&nbsp;PURPOSE.&nbsp;&nbsp;See&nbsp;the</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;GNU&nbsp;General&nbsp;Public&nbsp;License&nbsp;for&nbsp;more&nbsp;details.</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;Load&nbsp;the&nbsp;required&nbsp;libraries</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>library(ggplot2)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>library("grid")</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;!!!&nbsp;CONFIGURE&nbsp;YOUR&nbsp;PLOT&nbsp;HERE&nbsp;!!!</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;Output</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_output&nbsp;&lt;-&nbsp;paste("/Users/AlgaeLab/Desktop/LIZ/BUSCO/plot_data/","busco_figure.png",sep="/")</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_width&nbsp;&lt;-&nbsp;20</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_height&nbsp;&lt;-&nbsp;15</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_unit&nbsp;&lt;-&nbsp;"cm"</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;Colors</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_colors&nbsp;&lt;-&nbsp;c("#56B4E9",&nbsp;"#3492C7",&nbsp;"#F0E442",&nbsp;"#F04442")</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;Bar&nbsp;height&nbsp;ratio</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_bar_height&nbsp;&lt;-&nbsp;0.75</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;Legend</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_title&nbsp;&lt;-&nbsp;"BUSCO&nbsp;Assessment&nbsp;Results"</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;Font</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_family&nbsp;&lt;-&nbsp;"sans"</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_size_ratio&nbsp;&lt;-&nbsp;1</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;!!!&nbsp;SEE&nbsp;YOUR&nbsp;DATA&nbsp;HERE&nbsp;!!!</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;Your&nbsp;data&nbsp;as&nbsp;generated&nbsp;by&nbsp;python,&nbsp;remove&nbsp;or&nbsp;add&nbsp;more</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_species&nbsp;&lt;-&nbsp;c('cardio',&nbsp;'cardio',&nbsp;'cardio',&nbsp;'cardio',&nbsp;'neph',&nbsp;'neph',&nbsp;'neph',&nbsp;'neph')</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_species&nbsp;&lt;-&nbsp;factor(my_species)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_species&nbsp;&lt;-&nbsp;factor(my_species,levels(my_species)[c(length(levels(my_species)):1)])&nbsp;#&nbsp;reorder&nbsp;your&nbsp;species&nbsp;here&nbsp;just&nbsp;by&nbsp;changing&nbsp;the&nbsp;values&nbsp;in&nbsp;the&nbsp;vector&nbsp;:</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_percentage&nbsp;&lt;-&nbsp;c(15.8,&nbsp;33.3,&nbsp;0.0,&nbsp;50.9,&nbsp;6.4,&nbsp;39.3,&nbsp;1.3,&nbsp;53.0)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>my_values&nbsp;&lt;-&nbsp;c(37,&nbsp;78,&nbsp;0,&nbsp;119,&nbsp;15,&nbsp;92,&nbsp;3,&nbsp;124)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>######################################</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>######################################</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>######################################</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#&nbsp;Code&nbsp;to&nbsp;produce&nbsp;the&nbsp;graph</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>labsize&nbsp;=&nbsp;1</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>if&nbsp;(length(levels(my_species))&nbsp;&gt;&nbsp;10){</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;labsize&nbsp;=&nbsp;0.66</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>}</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>print("Plotting&nbsp;the&nbsp;figure&nbsp;...")</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>category&nbsp;&lt;-&nbsp;c(rep(c("S","D","F","M"),c(1)))</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>category&nbsp;&lt;-factor(category)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>category&nbsp;=&nbsp;factor(category,levels(category)[c(4,1,2,3)])</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>df&nbsp;=&nbsp;data.frame(my_species,my_percentage,my_values,category)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>figure&nbsp;&lt;-&nbsp;ggplot()&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;geom_bar(aes(y&nbsp;=&nbsp;my_percentage,&nbsp;x&nbsp;=&nbsp;my_species,&nbsp;fill&nbsp;=&nbsp;category),&nbsp;data&nbsp;=&nbsp;df,&nbsp;stat="identity",&nbsp;width=my_bar_height)&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;coord_flip()&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme_gray(base_size&nbsp;=&nbsp;8)&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;scale_y_continuous(labels&nbsp;=&nbsp;c("0","20","40","60","80","100"),&nbsp;breaks&nbsp;=&nbsp;c(0,20,40,60,80,100))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;scale_fill_manual(values&nbsp;=&nbsp;my_colors,labels&nbsp;=c("&nbsp;Complete&nbsp;(C)&nbsp;and&nbsp;single-copy&nbsp;(S)&nbsp;&nbsp;",</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"&nbsp;Complete&nbsp;(C)&nbsp;and&nbsp;duplicated&nbsp;(D)",</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"&nbsp;Fragmented&nbsp;(F)&nbsp;&nbsp;",</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"&nbsp;Missing&nbsp;(M)"))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;ggtitle(my_title)&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;xlab("")&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;ylab("\n%BUSCOs")&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(plot.title&nbsp;=&nbsp;element_text(family=my_family,&nbsp;colour&nbsp;=&nbsp;"black",&nbsp;size&nbsp;=&nbsp;rel(2.2)*my_size_ratio,&nbsp;face&nbsp;=&nbsp;"bold"))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(legend.position="top",legend.title&nbsp;=&nbsp;element_blank())&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(legend.text&nbsp;=&nbsp;element_text(family=my_family,&nbsp;size&nbsp;=&nbsp;rel(1.2)*my_size_ratio))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(panel.background&nbsp;=&nbsp;element_rect(color="#FFFFFF",&nbsp;fill="white"))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(panel.grid.minor&nbsp;=&nbsp;element_blank())&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(panel.grid.major&nbsp;=&nbsp;element_blank())&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(axis.text.y&nbsp;=&nbsp;element_text(family=my_family,&nbsp;colour&nbsp;=&nbsp;"black",&nbsp;size&nbsp;=&nbsp;rel(1.66)*my_size_ratio))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(axis.text.x&nbsp;=&nbsp;element_text(family=my_family,&nbsp;colour&nbsp;=&nbsp;"black",&nbsp;size&nbsp;=&nbsp;rel(1.66)*my_size_ratio))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(axis.line&nbsp;=&nbsp;element_line(size=1*my_size_ratio,&nbsp;colour&nbsp;=&nbsp;"black"))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(axis.ticks.length&nbsp;=&nbsp;unit(.85,&nbsp;"cm"))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(axis.ticks.y&nbsp;=&nbsp;element_line(colour="white",&nbsp;size&nbsp;=&nbsp;0))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(axis.ticks.x&nbsp;=&nbsp;element_line(colour="#222222"))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(axis.ticks.length&nbsp;=&nbsp;unit(0.4,&nbsp;"cm"))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;theme(axis.title.x&nbsp;=&nbsp;element_text(family=my_family,&nbsp;size=rel(1.2)*my_size_ratio))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;guides(fill&nbsp;=&nbsp;guide_legend(override.aes&nbsp;=&nbsp;list(colour&nbsp;=&nbsp;NULL)))&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;guides(fill=guide_legend(nrow=2,byrow=TRUE))</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;for(i&nbsp;in&nbsp;rev(c(1:length(levels(my_species))))){</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;&nbsp;&nbsp;detailed_values&nbsp;&lt;-&nbsp;my_values[my_species==my_species[my_species==levels(my_species)[i]]]</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;&nbsp;&nbsp;total_buscos&nbsp;&lt;-&nbsp;sum(detailed_values)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;&nbsp;&nbsp;figure&nbsp;&lt;-&nbsp;figure&nbsp;+</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;&nbsp;&nbsp;annotate("text",&nbsp;label=paste("C:",&nbsp;detailed_values[1]&nbsp;+&nbsp;detailed_values[2],&nbsp;"&nbsp;[S:",&nbsp;detailed_values[1],&nbsp;",&nbsp;D:",&nbsp;detailed_values[2],&nbsp;"],&nbsp;F:",&nbsp;detailed_values[3],&nbsp;",&nbsp;M:",&nbsp;detailed_values[4],&nbsp;",&nbsp;n:",&nbsp;total_buscos,&nbsp;sep=""),</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y=3,&nbsp;x&nbsp;=&nbsp;i,&nbsp;size&nbsp;=&nbsp;labsize*4*my_size_ratio,&nbsp;colour&nbsp;=&nbsp;"black",&nbsp;hjust=0,&nbsp;family=my_family)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;&nbsp;}</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>ggsave(figure,&nbsp;file=my_output,&nbsp;width&nbsp;=&nbsp;my_width,&nbsp;height&nbsp;=&nbsp;my_height,&nbsp;unit&nbsp;=&nbsp;my_unit)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>print("Done")</span></span></div></pre><p><img alt="" src="/Users/lizhunter/Downloads/busco_figure.png"></p>
<h2 id="orthofinder">Orthofinder</h2>
<p>Pull transcriptomes from eupath.db</p>
<ul>
<li>Toxoplasma gondii M64</li>
<li>Plasmodium falciparum 3D7</li>
<li>Cryptopsporidium parvum</li>
<li>Chromera velia</li>
</ul>
<p>Combined with assembled transcriptomes</p>
<ul>
<li>Nephromyces isolate</li>
<li>Cardiosporidium cionae</li>
</ul>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>conda&nbsp;install&nbsp;-c&nbsp;bioconda&nbsp;orthofinder</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>mkdir&nbsp;Orthofinder</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>mv&nbsp;*.fasta&nbsp;/Orthofinder</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>orthofinder&nbsp;-f&nbsp;orthofinder/&nbsp;-t&nbsp;5</span></span></div></pre><p>OrthoFinder assigned 70927 genes (64.8% of total) to 6422 orthogroups. Fifty percent of all genes were in orthogroups with 9 or more genes (G50 was 9) and were contained in the largest 2742 orthogroups (O50 was 2742). There were 1341 orthogroups with all species present and 4 of these consisted entirely of single-copy genes.</p>
<h4 id="tree-generated-by-orthofinder">Tree generated by OrthoFinder</h4>
<p><img alt="" src="/Users/lizhunter/Downloads/tree.png"></p>
<h2 id="goslim-analysis">GOSlim Analysis</h2>
<p>#sort Orthogroups.GeneCount.csv for orthologs contained in all groups (not just single copy)</p>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#Remove&nbsp;rows&nbsp;when&nbsp;there&nbsp;is&nbsp;a&nbsp;0&nbsp;in&nbsp;any&nbsp;column</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>Find&nbsp;and&nbsp;replace&nbsp;with&nbsp;nothing:&nbsp;^OG(.+)\t0t(.+)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#Remove&nbsp;blank&nbsp;lines</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>grep&nbsp;'[^[:blank:]]'&nbsp;&lt;&nbsp;orthos.fasta&nbsp;&gt;&nbsp;orthos2.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#Pull&nbsp;headers&nbsp;only</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>Find:&nbsp;^OG(\d+)\t(.+)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>Replace:&nbsp;OG\1</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#Pull&nbsp;sequences&nbsp;IDs&nbsp;from&nbsp;main&nbsp;ortho&nbsp;file</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>grep&nbsp;-F&nbsp;-w&nbsp;-f&nbsp;orthos3.tsv&nbsp;Orthogroups.tsv&nbsp;&gt;&nbsp;sharedseq.tsv</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#Sort&nbsp;for&nbsp;single&nbsp;(model)&nbsp;organism&nbsp;-&nbsp;used&nbsp;Toxoplasma</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>grep&nbsp;"Toxo"&nbsp;sharedseq.tsv&nbsp;&gt;&nbsp;toxoorthogroups.txt</span></span></div></pre><p>#Search genes on eupath.db and download GOterms</p>
<p>#Agbase to convert from GOterms to GOslim</p>
<p><img alt="" src="/Users/lizhunter/Downloads/image.png"></p>
<h2 id="virulence-factor-database">Virulence Factor Database</h2>
<ol>
<li>List of virulence factors from Kegg infectious disease pathway modules</li>
<li>Sequences for virulence factors found &amp; downloaded from eupath.db</li>
<li>List of all common virulence factors used as a blast database for the two assembled transcriptomes</li>
</ol>
<pre class="editor-colors lang-"><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#make&nbsp;database</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>makeblastdb&nbsp;-in&nbsp;virulencefactors.txt&nbsp;-parse_seqids&nbsp;-dbtype&nbsp;prot</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#run&nbsp;local&nbsp;blast</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>blastp&nbsp;-query&nbsp;trinity.fasta&nbsp;-db&nbsp;virulencefactors.fasta&nbsp;-outfmt&nbsp;6&nbsp;-max_target_seqs&nbsp;3&nbsp;&gt;&nbsp;nephvirulence.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#delete&nbsp;to&nbsp;header</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>Find:&nbsp;(T.+\|m\.\d+)\t.+\n</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>Replace:&nbsp;\1\n</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#pull&nbsp;sequences&nbsp;from&nbsp;translated&nbsp;protein&nbsp;file</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>grep&nbsp;-A1&nbsp;-w&nbsp;-f&nbsp;nephvirulence2.fasta&nbsp;nephvirulenceseq.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#delete&nbsp;duplicates</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>mothur&nbsp;uniq_seq</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#split&nbsp;into&nbsp;batches&nbsp;of&nbsp;100&nbsp;sequences</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>mkdir&nbsp;nephvirulence</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>awk&nbsp;'BEGIN&nbsp;{n_seq=0;}&nbsp;/^&gt;/&nbsp;{if(n_seq%100==0){file=sprintf("%d.fa",n_seq);}&nbsp;print&nbsp;&gt;&gt;&nbsp;file;&nbsp;n_seq++;&nbsp;next;}&nbsp;{&nbsp;print&nbsp;&gt;&gt;&nbsp;file;&nbsp;close(file)}'&nbsp;&lt;&nbsp;../nephvirulenceseq.fasta</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#rename&nbsp;sequentially&nbsp;(1-296)</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>n=1;&nbsp;for&nbsp;x&nbsp;in&nbsp;*.fa;&nbsp;do&nbsp;mv&nbsp;$x&nbsp;&nbsp;$n.fa;&nbsp;n=$(($n+1));&nbsp;done</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#array&nbsp;blast&nbsp;on&nbsp;bluewaves</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#!/bin/bash</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#SBATCH&nbsp;-J&nbsp;blast</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#SBATCH&nbsp;-t&nbsp;10:00:00</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#SBATCH&nbsp;-N&nbsp;1</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#SBATCH&nbsp;-n&nbsp;16</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#SBATCH&nbsp;--array=1-296</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>module&nbsp;load&nbsp;blast</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>blastp&nbsp;-db&nbsp;/data3/shared/ncbi-refseq_protein/refseq_protein.36&nbsp;\</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>-query&nbsp;"$SLURM_ARRAY_TASK_ID".fa&nbsp;\</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>-out&nbsp;"$SLURM_ARRAY_TASK_ID".out&nbsp;\</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>-outfmt&nbsp;'6&nbsp;qseqid&nbsp;sseqid'&nbsp;\</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>-max_target_seqs&nbsp;1&nbsp;\</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>-num_threads&nbsp;16</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#pull&nbsp;GI&nbsp;numbers</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>Find:&nbsp;.+gi\|(\d+)\|.+\n</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>Replace:&nbsp;\1\n</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#split&nbsp;into&nbsp;smaller&nbsp;files</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>split&nbsp;-l&nbsp;2500&nbsp;nephblast.txt</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>&nbsp;</span></span></div><div class="line"><span class="syntax--text syntax--plain syntax--null-grammar"><span>#run&nbsp;on&nbsp;NCBI&nbsp;batch&nbsp;entrez</span></span></div></pre><p>(this last piece ended up giving a ton of noise and not anything worth using, need to find a better way to filter these results, perhaps a smaller more specific blast database)</p></body>
</html>
