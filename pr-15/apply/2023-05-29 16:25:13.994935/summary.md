# IAMbic Summary
## Change Detection
* 2 distinct actions.
* 8 templates with changes.
* 1 accounts affected.
## Exceptions
* 0 exceptions were recorded.

# IAMbic Change Details

<details>
<summary>Action: Create (Number of Templates: 4)</summary>
    <blockquote>
        <details>
        <summary>Template: prevent_imdsv1.yaml (Number of Accounts: 1)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>PreventIMDSV1</td>
                                    <td>aws:iam:scp_policy:properties</td>
                                    <td>Create</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        <details>
        <summary>Template: prevent_root_login.yaml (Number of Accounts: 1)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>DontRootMe</td>
                                    <td>aws:iam:scp_policy:properties</td>
                                    <td>Create</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        <details>
        <summary>Template: restrict_regions.yaml (Number of Accounts: 1)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>RestrictRegions</td>
                                    <td>aws:iam:scp_policy:properties</td>
                                    <td>Create</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        <details>
        <summary>Template: prevent_disable_security_services.yaml (Number of Accounts: 1)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>PreventDisableSecurityServices</td>
                                    <td>aws:iam:scp_policy:properties</td>
                                    <td>Create</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        </blockquote>
</details>
<details>
<summary>Action: Attach (Number of Templates: 4)</summary>
    <blockquote>
        <details>
        <summary>Template: prevent_imdsv1.yaml (Number of Accounts: 1)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>None</td>
                                    <td>aws:iam:scp_policy:properties</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        <details>
        <summary>Template: restrict_regions.yaml (Number of Accounts: 1)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>None</td>
                                    <td>aws:iam:scp_policy:properties</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        <details>
        <summary>Template: prevent_root_login.yaml (Number of Accounts: 1)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>None</td>
                                    <td>aws:iam:scp_policy:properties</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        <details>
        <summary>Template: prevent_disable_security_services.yaml (Number of Accounts: 1)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>None</td>
                                    <td>aws:iam:scp_policy:properties</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        </blockquote>
</details>

