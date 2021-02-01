## API Report File for "firebase-admin.app"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { Agent } from 'http';

// @public (undocumented)
export interface App {
    name: string;
    options: AppOptions;
}

// @public (undocumented)
export function applicationDefault(httpAgent?: Agent): Credential;

// @public
export interface AppOptions {
    credential?: Credential;
    databaseAuthVariableOverride?: object | null;
    databaseURL?: string;
    httpAgent?: Agent;
    projectId?: string;
    serviceAccountId?: string;
    storageBucket?: string;
}

// @public (undocumented)
export function cert(serviceAccountPathOrObject: string | ServiceAccount, httpAgent?: Agent): Credential;

// @public (undocumented)
export interface Credential {
    getAccessToken(): Promise<GoogleOAuthAccessToken>;
}

// @public (undocumented)
export function deleteApp(app: App): Promise<void>;

// @public (undocumented)
export function getApp(name?: string): App;

// @public (undocumented)
export function getApps(): App[];

// @public
export interface GoogleOAuthAccessToken {
    // (undocumented)
    access_token: string;
    // (undocumented)
    expires_in: number;
}

// @public (undocumented)
export function initializeApp(options?: AppOptions, name?: string): App;

// @public (undocumented)
export function refreshToken(refreshTokenPathOrObject: string | object, httpAgent?: Agent): Credential;

// @public (undocumented)
export const SDK_VERSION: string;

// @public (undocumented)
export interface ServiceAccount {
    // (undocumented)
    clientEmail?: string;
    // (undocumented)
    privateKey?: string;
    // (undocumented)
    projectId?: string;
}


// (No @packageDocumentation comment for this package)

```