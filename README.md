While GitHub supports Mermaid natively in their own Markdown previews,
the default GitHub Pages action (which uses Jekyll) does not render Mermaid blocks.

This small repo shows how to configure the used Jekyll layout to render Mermaid diagrams.

The script gets triggered if `language-mermaid` appears in the output,
which is the class name Jekyll uses for rendered Mermaid code blocks.

The Mermaid module is loaded via JSDelivr with subresource integrity in place.
This is achieved by preloading the module with the hash stated (unless you use an old browser).
