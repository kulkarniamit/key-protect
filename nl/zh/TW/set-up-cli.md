---

copyright:
  years: 2017, 2019
lastupdated: "2019-01-03"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:important: .important}

# 設定 CLI
{: #set-up-cli}

您可以使用 {{site.data.keyword.keymanagementservicelong_notm}} CLI 外掛程式，以協助您建立、匯入及管理加密金鑰。

若要進一步了解如何使用 CLI，請參閱 [{{site.data.keyword.keymanagementserviceshort}} CLI 參考資料文件](/docs/services/key-protect/cli-reference.html)。
{: tip}

## 安裝 {{site.data.keyword.keymanagementserviceshort}} CLI 外掛程式
{: #install-cli}

請先安裝 [{{site.data.keyword.cloud_notm}} CLI ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](/docs/cli/index.html#overview){: new_window}，然後才能設定 {{site.data.keyword.keymanagementserviceshort}} CLI 外掛程式。 

若要安裝 CLI，請執行下列動作：

1. 安裝 [{{site.data.keyword.cloud_notm}} CLI ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](/docs/cli/index.html#overview){: new_window}。

    安裝 CLI 之後，您可以執行 `ibmcloud` 指令，與雲端服務互動。

2. 登入 {{site.data.keyword.cloud_notm}}。

    ```sh
    ibmcloud login
    ```
    {: pre}

    **附註：**如果登入失敗，請執行 `ibmcloud login --sso` 指令再試一次。當您使用聯合 ID 登入時，需要 `--sso` 參數。如果使用這個選項，請前往 CLI 輸出中所列的鏈結，以產生一次性的通行碼。

3. 若要開始管理加密金鑰，請安裝 {{site.data.keyword.keymanagementserviceshort}} CLI 外掛程式。

    ```sh
    ibmcloud plugin install key-protect -r 'IBM Cloud'
    ```
    {: pre}

4. 選用項目：確認已順利安裝外掛程式。

    ```sh
    ibmcloud plugin list
    ```
    {: pre}

## 更新 {{site.data.keyword.keymanagementserviceshort}} CLI 外掛程式
{: #update-cli}

建議您定期更新 CLI 以使用新特性。

若要更新 CLI，請執行下列動作：

1. 使用 [{{site.data.keyword.cloud_notm}} CLI ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](/docs/cli/index.html#overview){: new_window}，登入 {{site.data.keyword.cloud_notm}}。

    ```sh
    ibmcloud login 
    ```
    {: pre}

    **附註：**如果登入失敗，請執行 `ibmcloud login --sso` 指令再試一次。當您使用聯合 ID 登入時，需要 `--sso` 參數。如果使用這個選項，請前往 CLI 輸出中所列的鏈結，以產生一次性的通行碼。

2. 從外掛程式儲存庫安裝更新。

    ```sh
    ibmcloud plugin update key-protect -r 'IBM Cloud'
    ```
    {: pre}

3. 選用項目：確認已順利更新外掛程式。

    ```sh
    ibmcloud plugin list
    ```
    {: pre}

## 解除安裝 {{site.data.keyword.keymanagementserviceshort}} CLI 外掛程式
{: #uninstall-cli}

1. 使用 [{{site.data.keyword.cloud_notm}} CLI ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](/docs/cli/index.html#overview){: new_window}，登入 {{site.data.keyword.cloud_notm}}。

    ```sh
    ibmcloud login 
    ```
    {: pre}

    **附註：**如果登入失敗，請執行 `ibmcloud login --sso` 指令再試一次。當您使用聯合 ID 登入時，需要 `--sso` 參數。如果使用這個選項，請前往 CLI 輸出中所列的鏈結，以產生一次性的通行碼。

2. 從外掛程式儲存庫安裝更新。

    ```sh
    ibmcloud plugin uninstall key-protect
    ```
    {: pre}

3. 選用項目：確認已順利解除安裝外掛程式。

    ```sh
    ibmcloud plugin list
    ```
    {: pre}