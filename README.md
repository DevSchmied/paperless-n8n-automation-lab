# Paperless n8n Automation Lab

This repository documents a lab setup for automating Paperless-ngx workflows with n8n.

## Goal

The goal is to test how Paperless-ngx can trigger an n8n workflow after document processing.

The n8n workflow receives a document ID, calls the Paperless API, retrieves document metadata and sends a Telegram notification.

## Workflow

```text
Paperless-ngx
↓
Post-consume script / webhook call
↓
n8n Webhook
↓
HTTP Request to Paperless API
↓
Telegram notification