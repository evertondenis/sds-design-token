# SDS Design Tokens

<!--[![npm version](https://img.shields.io/badge/npm-v0.0.8-green.svg)](https://www.npmjs.com/package/sds-design-token)--->

SDS Design Tokens is an experimental project to generate design-tokens to create UI components with some base specific design system

## Getting Started

```sh
npm i sds-design-token --save
```

```sh
yarn add sds-design-token
```

## Usage

Example with styled-components:

```jsx
import styled from 'styled-components';
import {
  Animations,
  Borders,
  Colors,
  Spacings,
  Typography
} from 'sds-design-token';

export const Button = styled.button`
  background: ${Colors.colorPrimary};
  border: 0;
  border-radius: ${Borders.borderRadius};
  color: ${Colors.colorWhitePrimary};
  cursor: pointer;
  font-family: ${Typography.fontFamilyPrimary};
  font-size: ${Typography.fontSizeBase};
  padding: ${Spacings.spacingBase};
  transition: all ${Animations.durationSm} ${Animations.timingBase};

  &:hover {
    background: ${Colors.colorPrimaryLight};
  }
`;
```

**Take a look at this working example at** [codesandbox.io](https://codesandbox.io/s/y21k4l9729)

## Properties

### Colors

| Attributes            | Values                   |
| --------------------- | ------------------------ |
| colorWarning          | rgb(228, 126, 26)        |
| colorBackgroundLight  | rgb(245, 245, 245)       |
| colorWhiteSecondary   | rgba(255, 255, 255, 0.6) |
| colorBlack            | rgb(0, 0, 0)             |
| colorPrimary          | rgb(0, 91, 149)          |
| colorBlackPrimary     | rgba(0, 0, 0, 0.87)      |
| colorSuccess          | rgb(90, 153, 48)         |
| colorBackgroundMedium | rgb(238, 238, 238)       |
| colorBackgroundDark   | rgb(221, 221, 221)       |
| colorError            | rgb(176, 0, 32)          |
| colorPrimaryMedium    | rgb(8, 140, 202)         |
| colorSecondaryLight   | rgb(241, 241, 241)       |
| colorWhitePrimary     | rgb(255, 255, 255)       |
| colorSecondary        | rgb(71, 71, 71)          |
| colorBlackSecondary   | rgba(0, 0, 0, 0.6)       |
| colorSecondaryMedium  | rgb(102, 102, 102)       |
| colorPrimaryLight     | rgb(132, 214, 245)       |
| colorSuport           | rgb(8, 140, 202)         |

### Typographies

| Attributes          | Values                 |
| ------------------- | ---------------------- |
| fontFamilyPrimary   | Open Sans, sans-serif  |
| fontFamilySecondary | Montserrat, sans-serif |
| fontSizeBase        | 1rem                   |
| fontSizeSm          | 0.875rem               |
| fontSizeXs          | 0.75rem                |
| lineHeightBase      | 1.5rem                 |
| lineHeightSm        | 1.25rem                |
| lineHeightXs        | 1rem                   |

### Spacings

| Attributes  | Values  |
| ----------- | ------- |
| spacingBase | 1rem    |
| spacingXl   | 2rem    |
| spacingXxl  | 2.5rem  |
| spacingMd   | 0.75rem |
| spacingNone | 0rem    |
| spacingSm   | 0.5rem  |
| spacingXs   | .25rem  |
| spacingLg   | 1.5rem  |
| spacingXxs  | .125rem |

### Borders

| Attributes             | Values                    |
| ---------------------- | ------------------------- |
| borderSizeMd           | 2px                       |
| colorBorderWhiteMedium | rgba(255, 255, 255, 0.38) |
| borderRadius           | 4px                       |
| borderSizeSm           | 1px                       |
| borderSizeLg           | 3px                       |
| colorBorderWhiteLight  | rgba(255, 255, 255, 0.2)  |
| colorBorderMedium      | rgba(0, 0, 0, 0.24)       |
| colorBorderDark        | rgba(0, 0, 0, 0.6)        |
| colorBorderLight       | rgba(0, 0, 0, 0.12)       |

### Opacities

| Attributes                     | Values |
| ------------------------------ | ------ |
| opacityBackgroundLightHover    | 0.04   |
| opacityBackgroundLightSelected | 0.08   |
| opacityBackgroundLightActive   | 0.24   |
| opacityBackgroundDarkHover     | 0.12   |
| opacityBackgroundDarkSelected  | 0.16   |
| opacityBackgroundDarkActive    | 0.24   |
| opacityDisabled                | 0.4    |

### Widths

| Attributes           | Values   |
| -------------------- | -------- |
| containerMaxWidth    | 74.75rem |
| containerMWidth      | 49rem    |
| containerSWidth      | 35rem    |
| containerXsWidth     | 17.5rem  |
| containerMobileWidth | 20rem    |

### MediaQueries ( breakpoints)

| Attributes       | Values |
| ---------------- | ------ |
| mediaQuerySmall  | 36rem  |
| mediaQueryMedium | 48rem  |
| mediaQueryLarge  | 62rem  |

### Animations

| Attributes   | Values   |
| ------------ | -------- |
| durationXs   | 100ms    |
| durationSm   | 200ms    |
| durationBase | 250ms    |
| timingBase   | ease-out |

<!---
#

Before run build, you need to give to permission to \*.sh file:

```sh
chmod +x scripts/start.sh
```
--->
