![Built Status](https://github.com/ddulic/damir.tech/workflows/setup-website/badge.svg)

# Website

- Built with [Hugo](https://gohugo.io), using the [hermit](https://themes.gohugo.io/hermit/) theme
- Hosted on AWS S3 with CloudFront
- Deployed with Github Workflows

# Resume

Used for the resume located @ https://damir.tech/resume

Triggers Github Workflow on commit and uses [markdown-resume](https://github.com/there4/markdown-resume) to generate the PDF.

Once the PDF is generated also generate the Markdown Resume for [damir.tech](https://github.com/ddulic/damir.tech).