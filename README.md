# Portfolio System 2020

A basic portfolio website for as close to free as you can get. WIP

## Features

- No-code setup
- Static files generated by [Eleventy](https://www.11ty.dev/), meaning it’s _fast_
- [TODO note about Netlify free hosting]
- [TODO Note about accessibility]
- Supports projects and posts (news, blog, etc.)
- [Netlify CMS](https://www.netlifycms.org/) for content editing

## Restrictions

TODO

- Can only support up to [todo] images
- Browser support
- Netlify Identity limits under free tier, https://www.netlify.com/pricing/#identity

## Getting Started

There are two ways to publish a website with this template depending on your technical skillset. Go down the [no-code setup](#) route if you’re not a developer or don’t want to deal with code. Go down the [advanced setup](#) route if you’re happy with `npm` and the command line.

### No-code setup

You don’t need to be a developer to get this site set up. All you need is a GitHub account, a Netlify account, and the ability to follow some instructions.

#### 1. Get a GitHub account

GitHub is a platform that stores code. Your website code and content are going to live on GitHub. If you have an account already, go ahead and log in. If not, sign up for an account. The free individual account is sufficient.

#### 2. Get a Netlify account

Netlify is a hosting provider that offers a generous free tier for people with static websites like this one. If you have a Netlify account, log in. If you don’t, sign up for one. It is _highly_ recommended that you use your GitHub account to sign up / in because it will make the Netlify CMS setup a lot simpler.

#### 3. Deploy this website

Click the button below to deploy this website to Netlify.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/sb-ph/portfolio-2020)

What this does is fork this repository, creating a duplicate version associated with your own GitHub account, and then it deploys your version to Netlify.

When you click the button, you’ll be asked to connect to GitHub. Go ahead and do that.

TODO add more info about what this does, how to find their site in Netlify

#### 4. Configure your site

To customize the site-wide information such as the footer text or the site title, edit `src/data/global.json`.

#### 5. Enable Netlify CMS

Netlify CMS is a content management system that will allow you to edit your content without editing code.

To get Netlify CMS working, we need to enable Netlify Identity and Git Gateway. Netlify Identity manages our users and logins, and Git Gateway manages the editorial connection between the CMS and the content which is stored in GitHub. Follow the Netlify documentation to [enable Netlify Identity and Git Gateway](https://www.netlifycms.org/docs/add-to-your-site/#enable-identity-and-git-gateway) or follow the instructions below.

To enable Netlify Identity, navigate to your new website within the Netlify admin area and then click the submenu item Identity. Click the button to enable Netlify Identity. Next, click the Settings button to access the settings and scroll down to Registration. Edit the registration preferences to Invite Only.

Next, scroll down to Services and then click the button Enable Git Gateway. This may open a popup window asking you to log in to GitHub if you aren’t already logged in, but it should enable itself automatically since we already connected our GitHub repo and Netlify instance in step 3.

Once you’ve set up Netlify Identity and Git Gateway, follow Netlify’s instructions to [access the CMS](https://www.netlifycms.org/docs/add-to-your-site/#accessing-the-cms). First you’ll add yourself as a user within the Netlify Identity admin area for your new website, and then you’ll be able to log in at `/admin` (`yoursite.com/admin`, for example).

#### 6. Hook up your domain

TODO

## Advanced setup

TODO

### Local Development

To run this locally, you need to install Node first. Once Node is installed, you can run these on the command line in the root of your project:

- `npm start`: starts development server
- `npm run build`: generates a production build
- `npm run debug`: runs eleventy with debug output

To customize the site, edit `src/data/meta.js` with your details, or set the corresponding environment variables in a new `.env` file in the root folder of the project.

## Extending the site

You’re welcome to tinker and extend your website however you please by following the Eleventy and Netlify CMS documentation. If you’re interested in our help, just get in touch and we’ll discuss options.

## Colophon

The docs are inspired by [Max Boeck’s Emergency Site](https://github.com/maxboeck/emergency-site).
