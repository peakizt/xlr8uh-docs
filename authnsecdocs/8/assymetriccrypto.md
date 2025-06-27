Directory structure:
└── digitalleaves-asymmetriccrypto/
    ├── README.md
    ├── LICENSE.txt
    ├── AsymmetricCrypto/
    │   ├── AppDelegate.swift
    │   ├── AsymmetricCrypto-Bridging-Header.h
    │   ├── AsymmetricCrypto.entitlements
    │   ├── AsymmetricCryptoManager.swift
    │   ├── Info.plist
    │   ├── UIViewController+Alerts.swift
    │   ├── ViewController.swift
    │   ├── Assets.xcassets/
    │   │   ├── Contents.json
    │   │   ├── AppIcon.appiconset/
    │   │   │   └── Contents.json
    │   │   └── background.imageset/
    │   │       └── Contents.json
    │   └── Base.lproj/
    │       ├── LaunchScreen.storyboard
    │       └── Main.storyboard
    └── AsymmetricCrypto.xcodeproj/
        ├── project.pbxproj
        ├── project.xcworkspace/
        │   └── contents.xcworkspacedata
        └── xcuserdata/
            └── Nacho.xcuserdatad/
                ├── xcdebugger/
                │   └── Breakpoints_v2.xcbkptlist
                └── xcschemes/
                    ├── AsymmetricCrypto.xcscheme
                    └── xcschememanagement.plist


Files Content:

================================================
FILE: README.md
================================================
# AsymmetricCryptoManager
AsymmetricCryptoManager is a Swift implementation of an asymmetric cryptography manager to facilitate the use of asymmetric cryptographic operations in Swift. Included is a sample view controller for testing purposes.

![](http://digitalleaves.com/wp-content/uploads/2015/10/ezgif.com-optimize.gif)

## Usage

AsymmetricCryptoManager follows the Singleton pattern, thus it must be accessed by means of the sharedInstance variable.

### Generating a key pair

```swift
AsymmetricCryptoManager.sharedInstance.createSecureKeyPair({ (success, error) -> Void in
  if success {
    // start using the key pair.
  } else {
    // handle the error
  }
})
```

### Encryption:

```swift
AsymmetricCryptoManager.sharedInstance.encryptMessageWithPublicKey(clearText) { (success, data, error) -> Void in
  if success {
    let b64encoded = data!.base64EncodedStringWithOptions([])
    // transmit b64encoded encrypted string.
  } else {
    // handle the error ...
  }
}
```

### Decryption:

```swift
AsymmetricCryptoManager.sharedInstance.decryptMessageWithPrivateKey(encryptedData) { (success, result, error) -> Void in
  if success {
    // manage the resulting string.
  } else {
    // manage the error
  }
```

### Sign a message:

```swift
AsymmetricCryptoManager.sharedInstance.signMessageWithPrivateKey(clearText) { (success, data, error) -> Void in
  if success {
    let b64encoded = data!.base64EncodedStringWithOptions([])
  } else {
    // manage the error
  }
}
```

### Verify the signature:

```swift
AsymmetricCryptoManager.sharedInstance.verifySignaturePublicKey(rawData, signatureData: signatureData) { (success, error) -> Void in
  if success {
    // verification was successful
  } else {
    // verification failed.
  }
}
```

## LICENSE

The MIT License (MIT)
Copyright (c) 2015 Ignacio Nieto Carvajal (http://digitalleaves.com)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.



================================================
FILE: LICENSE.txt
================================================
The MIT License (MIT)
Copyright (c) 2015 Ignacio Nieto Carvajal (http://digitalleaves.com)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


================================================
FILE: AsymmetricCrypto/AppDelegate.swift
================================================
//
//  AppDelegate.swift
//  AsymmetricCrypto
//
//  Created by Ignacio Nieto Carvajal on 4/10/15.
//  Copyright © 2015 Ignacio Nieto Carvajal. All rights reserved.
//

import UIKit

@UIApplicationMain
class AppDelegate: UIResponder, UIApplicationDelegate {

    var window: UIWindow?


    func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplicationLaunchOptionsKey: Any]?) -> Bool {
        // Override point for customization after application launch.
        return true
    }

    func applicationWillResignActive(_ application: UIApplication) {
        // Sent when the application is about to move from active to inactive state. This can occur for certain types of temporary interruptions (such as an incoming phone call or SMS message) or when the user quits the application and it begins the transition to the background state.
        // Use this method to pause ongoing tasks, disable timers, and throttle down OpenGL ES frame rates. Games should use this method to pause the game.
    }

    func applicationDidEnterBackground(_ application: UIApplication) {
        // Use this method to release shared resources, save user data, invalidate timers, and store enough application state information to restore your application to its current state in case it is terminated later.
        // If your application supports background execution, this method is called instead of applicationWillTerminate: when the user quits.
    }

    func applicationWillEnterForeground(_ application: UIApplication) {
        // Called as part of the transition from the background to the inactive state; here you can undo many of the changes made on entering the background.
    }

    func applicationDidBecomeActive(_ application: UIApplication) {
        // Restart any tasks that were paused (or not yet started) while the application was inactive. If the application was previously in the background, optionally refresh the user interface.
    }

    func applicationWillTerminate(_ application: UIApplication) {
        // Called when the application is about to terminate. Save data if appropriate. See also applicationDidEnterBackground:.
    }


}




================================================
FILE: AsymmetricCrypto/AsymmetricCrypto-Bridging-Header.h
================================================
//
//  Use this file to import your target's public headers that you would like to expose to Swift.
//

#import <CommonCrypto/CommonCrypto.h>


================================================
FILE: AsymmetricCrypto/AsymmetricCrypto.entitlements
================================================
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>keychain-access-groups</key>
	<array>
		<string>$(AppIdentifierPrefix)com.MyKeychainSharing.AsymmetricCrypto</string>
	</array>
</dict>
</plist>



================================================
FILE: AsymmetricCrypto/AsymmetricCryptoManager.swift
================================================
//
//  AsymmetricCryptoManager.swift
//  AsymmetricCrypto
//
//  Created by Ignacio Nieto Carvajal on 4/10/15.
//  Copyright © 2015 Ignacio Nieto Carvajal. All rights reserved.
//

import UIKit

// Singleton instance
private let _singletonInstance = AsymmetricCryptoManager()

// Constants
private let kAsymmetricCryptoManagerApplicationTag = "com.AsymmetricCrypto.keypair"
private let kAsymmetricCryptoManagerKeyType = kSecAttrKeyTypeRSA
private let kAsymmetricCryptoManagerKeySize = 2048
private let kAsymmetricCryptoManagerCypheredBufferSize = 1024
private let kAsymmetricCryptoManagerSecPadding: SecPadding = .PKCS1

enum AsymmetricCryptoException: Error {
    case unknownError
    case duplicateFoundWhileTryingToCreateKey
    case keyNotFound
    case authFailed
    case unableToAddPublicKeyToKeyChain
    case wrongInputDataFormat
    case unableToEncrypt
    case unableToDecrypt
    case unableToSignData
    case unableToVerifySignedData
    case unableToPerformHashOfData
    case unableToGenerateAccessControlWithGivenSecurity
    case outOfMemory
}

class AsymmetricCryptoManager: NSObject {

    /** Shared instance */
    class var sharedInstance: AsymmetricCryptoManager {
        return _singletonInstance
    }

    // MARK: - Manage keys

    func createSecureKeyPair(_ completion: ((_ success: Bool, _ error: AsymmetricCryptoException?) -> Void)? = nil) {
        // private key parameters
        let privateKeyParams: [String: AnyObject] = [
            kSecAttrIsPermanent as String: true as AnyObject,
            kSecAttrApplicationTag as String: kAsymmetricCryptoManagerApplicationTag as AnyObject
        ]

        // private key parameters
        let publicKeyParams: [String: AnyObject] = [
            kSecAttrIsPermanent as String: true as AnyObject,
            kSecAttrApplicationTag as String: kAsymmetricCryptoManagerApplicationTag as AnyObject
        ]

        // global parameters for our key generation
        let parameters: [String: AnyObject] = [
            kSecAttrKeyType as String:          kAsymmetricCryptoManagerKeyType,
            kSecAttrKeySizeInBits as String:    kAsymmetricCryptoManagerKeySize as AnyObject,
            kSecPublicKeyAttrs as String:       publicKeyParams as AnyObject,
            kSecPrivateKeyAttrs as String:      privateKeyParams as AnyObject,
        ]

        // asynchronously generate the key pair and call the completion block
        DispatchQueue.global(qos: DispatchQoS.QoSClass.default).async { () -> Void in
            var pubKey, privKey: SecKey?
            let status = SecKeyGeneratePair(parameters as CFDictionary, &pubKey, &privKey)

            if status == errSecSuccess {
                DispatchQueue.main.async(execute: { completion?(true, nil) })
            } else {
                var error = AsymmetricCryptoException.unknownError
                switch (status) {
                case errSecDuplicateItem: error = .duplicateFoundWhileTryingToCreateKey
                case errSecItemNotFound: error = .keyNotFound
                case errSecAuthFailed: error = .authFailed
                default: break
                }
                DispatchQueue.main.async(execute: { completion?(false, error) })
            }
        }
    }

    func getPublicKeyData() -> Data? {
        let parameters = [
            kSecClass as String: kSecClassKey,
            kSecAttrKeyType as String: kSecAttrKeyTypeRSA,
            kSecAttrApplicationTag as String: kAsymmetricCryptoManagerApplicationTag,
            kSecAttrKeyClass as String: kSecAttrKeyClassPublic,
            kSecReturnData as String: true
        ] as [String : Any]
        var data: AnyObject?
        let status = SecItemCopyMatching(parameters as CFDictionary, &data)
        if status == errSecSuccess {
            return data as? Data
        } else { return nil }
    }

    func getPublicKeyReference() -> SecKey? {
        let parameters = [
            kSecClass as String: kSecClassKey,
            kSecAttrKeyType as String: kSecAttrKeyTypeRSA,
            kSecAttrApplicationTag as String: kAsymmetricCryptoManagerApplicationTag,
            kSecAttrKeyClass as String: kSecAttrKeyClassPublic,
            kSecReturnRef as String: true,
        ] as [String : Any]
        var ref: AnyObject?
        let status = SecItemCopyMatching(parameters as CFDictionary, &ref)
        if status == errSecSuccess { return ref as! SecKey? } else { return nil }
    }

    func getPrivateKeyReference() -> SecKey? {
        let parameters = [
            kSecClass as String: kSecClassKey,
            kSecAttrKeyClass as String: kSecAttrKeyClassPrivate,
            kSecAttrApplicationTag as String: kAsymmetricCryptoManagerApplicationTag,
            kSecReturnRef as String: true,
        ] as [String : Any]
        var ref: AnyObject?
        let status = SecItemCopyMatching(parameters as CFDictionary, &ref)
        if status == errSecSuccess { return ref as! SecKey? } else { return nil }
    }

    func keyPairExists() -> Bool {
        return self.getPublicKeyData() != nil
    }

    func deleteSecureKeyPair(_ completion: ((_ success: Bool) -> Void)?) {
        // private query dictionary
        let deleteQuery = [
            kSecClass as String: kSecClassKey,
            kSecAttrApplicationTag as String: kAsymmetricCryptoManagerApplicationTag,
        ] as [String : Any]

        DispatchQueue.global(qos: DispatchQoS.QoSClass.default).async { () -> Void in
            let status = SecItemDelete(deleteQuery as CFDictionary) // delete private key
            DispatchQueue.main.async(execute: { completion?(status == errSecSuccess) })        }
    }

    // MARK: - Cypher and decypher methods

    func encryptMessageWithPublicKey(_ message: String, completion: @escaping (_ success: Bool, _ data: Data?, _ error: AsymmetricCryptoException?) -> Void) {
        DispatchQueue.global(qos: DispatchQoS.QoSClass.default).async { () -> Void in

            if let publicKeyRef = self.getPublicKeyReference() {
                // prepare input input plain text
                guard let messageData = message.data(using: String.Encoding.utf8) else {
                    completion(false, nil, .wrongInputDataFormat)
                    return
                }
                let plainText = (messageData as NSData).bytes.bindMemory(to: UInt8.self, capacity: messageData.count)
                let plainTextLen = messageData.count

                // prepare output data buffer
                var cipherData = Data(count: SecKeyGetBlockSize(publicKeyRef))
                let cipherText = cipherData.withUnsafeMutableBytes({ (bytes: UnsafeMutablePointer<UInt8>) -> UnsafeMutablePointer<UInt8> in
                    return bytes
                })
                var cipherTextLen = cipherData.count

                let status = SecKeyEncrypt(publicKeyRef, .PKCS1, plainText, plainTextLen, cipherText, &cipherTextLen)

                // analyze results and call the completion in main thread
                DispatchQueue.main.async(execute: { () -> Void in
                    completion(status == errSecSuccess, cipherData, status == errSecSuccess ? nil : .unableToEncrypt)
                    cipherText.deinitialize()
                })
                return
            } else { DispatchQueue.main.async(execute: { completion(false, nil, .keyNotFound) }) }
        }
    }

    func decryptMessageWithPrivateKey(_ encryptedData: Data, completion: @escaping (_ success: Bool, _ result: String?, _ error: AsymmetricCryptoException?) -> Void) {
        DispatchQueue.global(qos: DispatchQoS.QoSClass.default).async { () -> Void in

            if let privateKeyRef = self.getPrivateKeyReference() {
                // prepare input input plain text
                let encryptedText = (encryptedData as NSData).bytes.bindMemory(to: UInt8.self, capacity: encryptedData.count)
                let encryptedTextLen = encryptedData.count

                // prepare output data buffer
                var plainData = Data(count: kAsymmetricCryptoManagerCypheredBufferSize)
                let plainText = plainData.withUnsafeMutableBytes({ (bytes: UnsafeMutablePointer<UInt8>) -> UnsafeMutablePointer<UInt8> in
                    return bytes
                })
                var plainTextLen = plainData.count

                let status = SecKeyDecrypt(privateKeyRef, .PKCS1, encryptedText, encryptedTextLen, plainText, &plainTextLen)

                // analyze results and call the completion in main thread
                DispatchQueue.main.async(execute: { () -> Void in
                    if status == errSecSuccess {
                        // adjust NSData length
                        plainData.count = plainTextLen
                        // Generate and return result string
                        if let string = NSString(data: plainData as Data, encoding: String.Encoding.utf8.rawValue) as? String {
                            completion(true, string, nil)
                        } else { completion(false, nil, .unableToDecrypt) }
                    } else { completion(false, nil, .unableToDecrypt) }
                    plainText.deinitialize()
                })
                return
            } else { DispatchQueue.main.async(execute: { completion(false, nil, .keyNotFound) }) }
        }
    }

    // MARK: - Sign and verify signature.

    func signMessageWithPrivateKey(_ message: String, completion: @escaping (_ success: Bool, _ data: Data?, _ error: AsymmetricCryptoException?) -> Void) {
        DispatchQueue.global(qos: DispatchQoS.QoSClass.default).async { () -> Void in
            var error: AsymmetricCryptoException? = nil

            if let privateKeyRef = self.getPrivateKeyReference() {
                // result data
                var resultData = Data(count: SecKeyGetBlockSize(privateKeyRef))
                let resultPointer = resultData.withUnsafeMutableBytes({ (bytes: UnsafeMutablePointer<UInt8>) -> UnsafeMutablePointer<UInt8> in
                    return bytes
                })
                var resultLength = resultData.count

                if let plainData = message.data(using: String.Encoding.utf8) {
                    // generate hash of the plain data to sign
                    var hashData = Data(count: Int(CC_SHA1_DIGEST_LENGTH))
                    let hash = hashData.withUnsafeMutableBytes({ (bytes: UnsafeMutablePointer<UInt8>) -> UnsafeMutablePointer<UInt8> in
                        return bytes
                    })
                    CC_SHA1((plainData as NSData).bytes.bindMemory(to: Void.self, capacity: plainData.count), CC_LONG(plainData.count), hash)

                    // sign the hash
                    let status = SecKeyRawSign(privateKeyRef, SecPadding.PKCS1SHA1, hash, hashData.count, resultPointer, &resultLength)
                    if status != errSecSuccess { error = .unableToEncrypt }
                    else { resultData.count = resultLength }
                    hash.deinitialize()
                } else { error = .wrongInputDataFormat }

                // analyze results and call the completion in main thread
                DispatchQueue.main.async(execute: { () -> Void in
                    if error == nil {
                        // adjust NSData length and return result.
                        resultData.count = resultLength
                        completion(true, resultData as Data, nil)
                    } else { completion(false, nil, error) }
                    //resultPointer.destroy()
                })
            } else { DispatchQueue.main.async(execute: { completion(false, nil, .keyNotFound) }) }
        }
    }

    func verifySignaturePublicKey(_ data: Data, signatureData: Data, completion: @escaping (_ success: Bool, _ error: AsymmetricCryptoException?) -> Void) {
        DispatchQueue.global(qos: DispatchQoS.QoSClass.default).async { () -> Void in
            var error: AsymmetricCryptoException? = nil

            if let publicKeyRef = self.getPublicKeyReference() {
                // hash data
                var hashData = Data(count: Int(CC_SHA1_DIGEST_LENGTH))
                let hash = hashData.withUnsafeMutableBytes({ (bytes: UnsafeMutablePointer<UInt8>) -> UnsafeMutablePointer<UInt8> in
                    return bytes
                })
                CC_SHA1((data as NSData).bytes.bindMemory(to: Void.self, capacity: data.count), CC_LONG(data.count), hash)
                // input and output data
                let signaturePointer = (signatureData as NSData).bytes.bindMemory(to: UInt8.self, capacity: signatureData.count)
                let signatureLength = signatureData.count

                let status = SecKeyRawVerify(publicKeyRef, SecPadding.PKCS1SHA1, hash, Int(CC_SHA1_DIGEST_LENGTH), signaturePointer, signatureLength)

                if status != errSecSuccess { error = .unableToDecrypt }

                // analyze results and call the completion in main thread
                hash.deinitialize()
                DispatchQueue.main.async(execute: { () -> Void in
                    completion(status == errSecSuccess, error)
                })
                return
            } else { DispatchQueue.main.async(execute: { completion(false, .keyNotFound) }) }
        }
    }


}







================================================
FILE: AsymmetricCrypto/Info.plist
================================================
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>CFBundleDevelopmentRegion</key>
	<string>en</string>
	<key>CFBundleExecutable</key>
	<string>$(EXECUTABLE_NAME)</string>
	<key>CFBundleIdentifier</key>
	<string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
	<key>CFBundleInfoDictionaryVersion</key>
	<string>6.0</string>
	<key>CFBundleName</key>
	<string>$(PRODUCT_NAME)</string>
	<key>CFBundlePackageType</key>
	<string>APPL</string>
	<key>CFBundleShortVersionString</key>
	<string>1.0</string>
	<key>CFBundleSignature</key>
	<string>????</string>
	<key>CFBundleVersion</key>
	<string>1</string>
	<key>LSRequiresIPhoneOS</key>
	<true/>
	<key>UILaunchStoryboardName</key>
	<string>LaunchScreen</string>
	<key>UIMainStoryboardFile</key>
	<string>Main</string>
	<key>UIRequiredDeviceCapabilities</key>
	<array>
		<string>armv7</string>
	</array>
	<key>UISupportedInterfaceOrientations</key>
	<array>
		<string>UIInterfaceOrientationPortrait</string>
		<string>UIInterfaceOrientationLandscapeLeft</string>
		<string>UIInterfaceOrientationLandscapeRight</string>
	</array>
</dict>
</plist>



================================================
FILE: AsymmetricCrypto/UIViewController+Alerts.swift
================================================
//
//  UIViewController+Alerts.swift
//
//  Created by Ignacio Nieto Carvajal on 13/7/15.
//  Copyright (c) 2015 Ignacio Nieto Carvajal. All rights reserved.
//

import UIKit

var asymmetricCryptoAlert: UIAlertController?

extension UIViewController {
    func showAlertWithMessage(_ msg: String, completion: (() -> Void)? = nil) {
        let alert = UIAlertController(title: nil, message: msg, preferredStyle: .alert)
        alert.addAction(UIAlertAction(title: "Ok", style: .default, handler: nil))
        asymmetricCryptoAlert = alert
        self.present(alert, animated: true, completion: completion)
    }

    func showAlertWithFadingOutMessage(_ msg: String, completion: (() -> Void)? = nil) {
        asymmetricCryptoAlert = UIAlertController(title: nil, message: msg, preferredStyle: .alert)
        self.present(asymmetricCryptoAlert!, animated: true, completion: completion)
        Timer.scheduledTimer(timeInterval: 3.0, target: self, selector: #selector(UIViewController.dismissLoadingMessageAlert), userInfo: nil, repeats: false)
    }

    func showLoadingAlertMessage(_ completion: (() -> Void)?) {
        let finalMessage = "Loading...\n\n\n"
        asymmetricCryptoAlert = UIAlertController(title: finalMessage, message: nil, preferredStyle: .alert)
        let activityIndicator = UIActivityIndicatorView(activityIndicatorStyle: .whiteLarge)
        activityIndicator.color = UIColor.black
        activityIndicator.center = CGPoint(x: 130.5, y: 85.5)
        asymmetricCryptoAlert!.view.addSubview(activityIndicator)
        activityIndicator.startAnimating()

        self.present(asymmetricCryptoAlert!, animated: true) { () -> Void in
            if completion != nil {
                DispatchQueue.main.asyncAfter(deadline: DispatchTime.now() + Double(Int64(0.0 * Double(NSEC_PER_SEC))) / Double(NSEC_PER_SEC), execute: { () -> Void in
                    completion!()
                })
            }
        }
    }

    func dismissLoadingMessageAlert() {
        self.dismissMessageAlert(nil)
    }

    func dismissMessageAlert(_ completion: (() -> Void)? = nil) {
        self.dismiss(animated: true, completion: { () -> Void in
            asymmetricCryptoAlert = nil
            completion?()
        })
    }
}



================================================
FILE: AsymmetricCrypto/ViewController.swift
================================================
//
//  ViewController.swift
//  AsymmetricCrypto
//
//  Created by Ignacio Nieto Carvajal on 4/10/15.
//  Copyright © 2015 Ignacio Nieto Carvajal. All rights reserved.
//

import UIKit

class ViewController: UIViewController {
    // MARK: - outlets && buttons
    @IBOutlet weak var keyPairLabel: UILabel!
    @IBOutlet weak var keyPairButton: UIButton!

    @IBOutlet weak var clearTextTextfield: UITextField!
    @IBOutlet weak var cypherButton: UIButton!
    @IBOutlet weak var signButton: UIButton!
    @IBOutlet weak var cypheredTextTextfield: UITextField!
    @IBOutlet weak var decypherButton: UIButton!
    @IBOutlet weak var verifySignatureButton: UIButton!

    // data
    var keyPairExists = AsymmetricCryptoManager.sharedInstance.keyPairExists() {
        didSet {
            if keyPairExists {
                keyPairLabel.text = "A valid keypair is present"
                keyPairButton.setTitle("Delete keypair", for: UIControlState())
            } else {
                keyPairLabel.text = "No key pair present"
                keyPairButton.setTitle("Generate keypair", for: UIControlState())
            }
            signButton.isEnabled = keyPairExists
            cypherButton.isEnabled = keyPairExists
            verifySignatureButton.isEnabled = keyPairExists
            decypherButton.isEnabled = keyPairExists
        }
    }

    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
    }

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }

    override func viewWillAppear(_ animated: Bool) {
        super.viewWillAppear(animated)
        self.keyPairExists = AsymmetricCryptoManager.sharedInstance.keyPairExists()
    }

    // MARK: - button actions
    @IBAction func generateKeyPair(_ sender: AnyObject) {
        self.view.isUserInteractionEnabled = false
        if keyPairExists { // delete current key pair
            AsymmetricCryptoManager.sharedInstance.deleteSecureKeyPair({ (success) -> Void in
                if success {
                    self.showAlertWithFadingOutMessage("Keypair successfully deleted")
                    self.keyPairExists = false
                } else { self.showAlertWithFadingOutMessage("Error deleting keypair.") }
                self.view.isUserInteractionEnabled = true
            })
        } else { // generate keypair
            AsymmetricCryptoManager.sharedInstance.createSecureKeyPair({ (success, error) -> Void in
                if success {
                    self.showAlertWithFadingOutMessage("RSA-2048 keypair successfully generated.")
                    self.keyPairExists = true
                } else { self.showAlertWithFadingOutMessage("An error happened while generating a keypair: \(error)") }
                self.view.isUserInteractionEnabled = true
            })
        }
    }

    @IBAction func cypherText(_ sender: AnyObject) {
        // safety check.
        if clearTextTextfield.text!.isEmpty {
            self.showAlertWithFadingOutMessage("Please, insert a clear text in the upper textfield.")
            return
        }
        self.view.isUserInteractionEnabled = false
        self.cypheredTextTextfield.text = ""
        self.view.endEditing(true)
        AsymmetricCryptoManager.sharedInstance.encryptMessageWithPublicKey(clearTextTextfield.text!) { (success, data, error) -> Void in
            if success {
                let b64encoded = data!.base64EncodedString(options: [])
                self.cypheredTextTextfield.text = b64encoded
                self.clearTextTextfield.text = ""
            } else {
                self.showAlertWithFadingOutMessage("Error cyphering data: \(error)")
            }
            self.view.isUserInteractionEnabled = true
        }
    }

    @IBAction func signText(_ sender: AnyObject) {
        // safety check.
        if clearTextTextfield.text!.isEmpty {
            self.showAlertWithFadingOutMessage("Please, insert the text to be signed in the upper textfield.")
            return
        }
        self.view.isUserInteractionEnabled = false
        self.cypheredTextTextfield.text = ""
        self.view.endEditing(true)
        AsymmetricCryptoManager.sharedInstance.signMessageWithPrivateKey(clearTextTextfield.text!) { (success, data, error) -> Void in
            if success {
                let b64encoded = data!.base64EncodedString(options: [])
                self.cypheredTextTextfield.text = b64encoded
            } else {
                self.showAlertWithFadingOutMessage("Error signing message: \(error)")
            }
            self.view.isUserInteractionEnabled = true
        }
    }

    @IBAction func decypherText(_ sender: AnyObject) {
        // safety check.
        if cypheredTextTextfield.text!.isEmpty {
            self.showAlertWithFadingOutMessage("Please, insert a cyphered, base64 encoded text in the lower textfield.")
            return
        }
        guard let encryptedData = Data(base64Encoded: cypheredTextTextfield.text!, options: []) else {
            self.showAlertWithFadingOutMessage("Unable to base64 decode the input string.")
            return
        }
        self.view.isUserInteractionEnabled = false
        self.clearTextTextfield.text = ""
        self.view.endEditing(true)
        AsymmetricCryptoManager.sharedInstance.decryptMessageWithPrivateKey(encryptedData) { (success, result, error) -> Void in
            if success {
                self.clearTextTextfield.text = result!
                self.cypheredTextTextfield.text = ""
            } else {
                self.showAlertWithFadingOutMessage("Error decoding base64 string: \(error)")
            }
            self.view.isUserInteractionEnabled = true
        }
    }

    @IBAction func verifySignature(_ sender: AnyObject) {
        // safety checks.
        if clearTextTextfield.text!.isEmpty {
            self.showAlertWithFadingOutMessage("Please, insert a the text that was signed in the upper textfield.")
            return
        }
        if cypheredTextTextfield.text!.isEmpty {
            self.showAlertWithFadingOutMessage("Please, insert the generated signature in the lower textfield.")
            return
        }

        guard let rawData = clearTextTextfield.text?.data(using: String.Encoding.utf8), let signatureData = Data(base64Encoded: cypheredTextTextfield.text!, options: []) else {
            self.showAlertWithFadingOutMessage("Unable to decode or identify input data. Probably one of the input fields is corrupted.")
            return
        }
        self.view.isUserInteractionEnabled = false
        self.view.endEditing(true)
        AsymmetricCryptoManager.sharedInstance.verifySignaturePublicKey(rawData, signatureData: signatureData) { (success, error) -> Void in
            self.showAlertWithFadingOutMessage(success ? "Signature verification was successful." : "Error: the signature is not valid for the input text")
            self.view.isUserInteractionEnabled = true
        }
    }
}




================================================
FILE: AsymmetricCrypto/Assets.xcassets/Contents.json
================================================
{
  "info" : {
    "version" : 1,
    "author" : "xcode"
  }
}


================================================
FILE: AsymmetricCrypto/Assets.xcassets/AppIcon.appiconset/Contents.json
================================================
{
  "images" : [
    {
      "idiom" : "iphone",
      "size" : "29x29",
      "scale" : "2x"
    },
    {
      "idiom" : "iphone",
      "size" : "29x29",
      "scale" : "3x"
    },
    {
      "idiom" : "iphone",
      "size" : "40x40",
      "scale" : "2x"
    },
    {
      "idiom" : "iphone",
      "size" : "40x40",
      "scale" : "3x"
    },
    {
      "idiom" : "iphone",
      "size" : "60x60",
      "scale" : "2x"
    },
    {
      "idiom" : "iphone",
      "size" : "60x60",
      "scale" : "3x"
    }
  ],
  "info" : {
    "version" : 1,
    "author" : "xcode"
  }
}


================================================
FILE: AsymmetricCrypto/Assets.xcassets/background.imageset/Contents.json
================================================
{
  "images" : [
    {
      "idiom" : "universal",
      "filename" : "photo-1422875646231-2bd603874ea8.jpeg",
      "scale" : "1x"
    },
    {
      "idiom" : "universal",
      "scale" : "2x"
    },
    {
      "idiom" : "universal",
      "scale" : "3x"
    }
  ],
  "info" : {
    "version" : 1,
    "author" : "xcode"
  }
}


================================================
FILE: AsymmetricCrypto/Base.lproj/LaunchScreen.storyboard
================================================
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<document type="com.apple.InterfaceBuilder3.CocoaTouch.Storyboard.XIB" version="3.0" toolsVersion="8150" systemVersion="15A204g" targetRuntime="iOS.CocoaTouch" propertyAccessControl="none" useAutolayout="YES" launchScreen="YES" useTraitCollections="YES" initialViewController="01J-lp-oVM">
    <dependencies>
        <plugIn identifier="com.apple.InterfaceBuilder.IBCocoaTouchPlugin" version="8122"/>
    </dependencies>
    <scenes>
        <!--View Controller-->
        <scene sceneID="EHf-IW-A2E">
            <objects>
                <viewController id="01J-lp-oVM" sceneMemberID="viewController">
                    <layoutGuides>
                        <viewControllerLayoutGuide type="top" id="Llm-lL-Icb"/>
                        <viewControllerLayoutGuide type="bottom" id="xb3-aO-Qok"/>
                    </layoutGuides>
                    <view key="view" contentMode="scaleToFill" id="Ze5-6b-2t3">
                        <rect key="frame" x="0.0" y="0.0" width="600" height="600"/>
                        <autoresizingMask key="autoresizingMask" widthSizable="YES" heightSizable="YES"/>
                        <animations/>
                        <color key="backgroundColor" white="1" alpha="1" colorSpace="custom" customColorSpace="calibratedWhite"/>
                    </view>
                </viewController>
                <placeholder placeholderIdentifier="IBFirstResponder" id="iYj-Kq-Ea1" userLabel="First Responder" sceneMemberID="firstResponder"/>
            </objects>
            <point key="canvasLocation" x="53" y="375"/>
        </scene>
    </scenes>
</document>



================================================
FILE: AsymmetricCrypto/Base.lproj/Main.storyboard
================================================
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<document type="com.apple.InterfaceBuilder3.CocoaTouch.Storyboard.XIB" version="3.0" toolsVersion="8191" systemVersion="15A284" targetRuntime="iOS.CocoaTouch" propertyAccessControl="none" useAutolayout="YES" useTraitCollections="YES" initialViewController="BYZ-38-t0r">
    <dependencies>
        <plugIn identifier="com.apple.InterfaceBuilder.IBCocoaTouchPlugin" version="8154"/>
        <capability name="Constraints to layout margins" minToolsVersion="6.0"/>
    </dependencies>
    <scenes>
        <!--View Controller-->
        <scene sceneID="tne-QT-ifu">
            <objects>
                <viewController id="BYZ-38-t0r" customClass="ViewController" customModule="AsymmetricCrypto" customModuleProvider="target" sceneMemberID="viewController">
                    <layoutGuides>
                        <viewControllerLayoutGuide type="top" id="y3c-jy-aDJ"/>
                        <viewControllerLayoutGuide type="bottom" id="wfy-db-euE"/>
                    </layoutGuides>
                    <view key="view" contentMode="scaleToFill" id="8bC-Xf-vdC">
                        <rect key="frame" x="0.0" y="0.0" width="600" height="600"/>
                        <autoresizingMask key="autoresizingMask" widthSizable="YES" heightSizable="YES"/>
                        <subviews>
                            <imageView userInteractionEnabled="NO" alpha="0.20000000000000001" contentMode="scaleAspectFill" horizontalHuggingPriority="251" verticalHuggingPriority="251" image="background" translatesAutoresizingMaskIntoConstraints="NO" id="f1A-A8-4kJ">
                                <rect key="frame" x="0.0" y="0.0" width="600" height="600"/>
                                <animations/>
                            </imageView>
                            <label opaque="NO" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" text="Asymmetric Encryption" textAlignment="natural" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="7Oc-gW-REn">
                                <rect key="frame" x="176" y="28" width="249" height="32"/>
                                <animations/>
                                <fontDescription key="fontDescription" name="Futura-Medium" family="Futura" pointSize="24"/>
                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
                                <nil key="highlightedColor"/>
                            </label>
                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="Hxw-sy-EcD">
                                <rect key="frame" x="226" y="115" width="150" height="45"/>
                                <animations/>
                                <color key="backgroundColor" red="0.40000000600000002" green="0.80000001190000003" blue="1" alpha="1" colorSpace="calibratedRGB"/>
                                <constraints>
                                    <constraint firstAttribute="height" constant="45" id="Ukk-xM-rDz"/>
                                    <constraint firstAttribute="width" constant="150" id="ZQB-Oa-2bW"/>
                                </constraints>
                                <color key="tintColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
                                <state key="normal" title="Generate keypair"/>
                                <connections>
                                    <action selector="generateKeyPair:" destination="BYZ-38-t0r" eventType="touchUpInside" id="qld-lr-Y1X"/>
                                </connections>
                            </button>
                            <label opaque="NO" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" text="No key pair present" textAlignment="center" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="22w-oY-3kk">
                                <rect key="frame" x="223" y="84" width="155" height="23"/>
                                <animations/>
                                <fontDescription key="fontDescription" name="Futura-Medium" family="Futura" pointSize="17"/>
                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
                                <nil key="highlightedColor"/>
                            </label>
                            <label opaque="NO" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" text="Clear text" textAlignment="center" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="c1D-lJ-lUT">
                                <rect key="frame" x="262" y="200" width="76" height="23"/>
                                <animations/>
                                <fontDescription key="fontDescription" name="Futura-Medium" family="Futura" pointSize="17"/>
                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
                                <nil key="highlightedColor"/>
                            </label>
                            <textField opaque="NO" clipsSubviews="YES" contentMode="scaleToFill" contentHorizontalAlignment="left" contentVerticalAlignment="center" borderStyle="roundedRect" textAlignment="natural" minimumFontSize="17" translatesAutoresizingMaskIntoConstraints="NO" id="kkT-sX-2Lu">
                                <rect key="frame" x="20" y="231" width="560" height="30"/>
                                <animations/>
                                <fontDescription key="fontDescription" type="system" pointSize="14"/>
                                <textInputTraits key="textInputTraits"/>
                            </textField>
                            <label opaque="NO" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" text="Cyphered text / signature (Base64)" textAlignment="center" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="mvS-yU-sUC">
                                <rect key="frame" x="163" y="336" width="274" height="23"/>
                                <animations/>
                                <fontDescription key="fontDescription" name="Futura-Medium" family="Futura" pointSize="17"/>
                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
                                <nil key="highlightedColor"/>
                            </label>
                            <textField opaque="NO" clipsSubviews="YES" contentMode="scaleToFill" contentHorizontalAlignment="left" contentVerticalAlignment="center" borderStyle="roundedRect" textAlignment="natural" minimumFontSize="17" translatesAutoresizingMaskIntoConstraints="NO" id="TCy-Eu-9P5">
                                <rect key="frame" x="20" y="367" width="560" height="30"/>
                                <animations/>
                                <fontDescription key="fontDescription" type="system" pointSize="14"/>
                                <textInputTraits key="textInputTraits"/>
                            </textField>
                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="r36-YD-WXp">
                                <rect key="frame" x="20" y="405" width="120" height="45"/>
                                <animations/>
                                <color key="backgroundColor" red="0.50196081400000003" green="0.0" blue="1" alpha="1" colorSpace="calibratedRGB"/>
                                <constraints>
                                    <constraint firstAttribute="height" constant="45" id="PGj-GA-Eaz"/>
                                    <constraint firstAttribute="width" constant="120" id="qit-WO-c1t"/>
                                </constraints>
                                <color key="tintColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
                                <state key="normal" title="Decypher"/>
                                <connections>
                                    <action selector="decypherText:" destination="BYZ-38-t0r" eventType="touchUpInside" id="3bs-5H-Jwg"/>
                                </connections>
                            </button>
                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="kla-S3-7i3">
                                <rect key="frame" x="460" y="405" width="120" height="45"/>
                                <animations/>
                                <color key="backgroundColor" red="0.80000001190000003" green="0.40000000600000002" blue="1" alpha="1" colorSpace="calibratedRGB"/>
                                <constraints>
                                    <constraint firstAttribute="height" constant="45" id="VY7-Gy-DWI"/>
                                    <constraint firstAttribute="width" constant="120" id="eul-YL-AV1"/>
                                </constraints>
                                <color key="tintColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
                                <state key="normal" title="Verify signature"/>
                                <connections>
                                    <action selector="verifySignature:" destination="BYZ-38-t0r" eventType="touchUpInside" id="RRt-bK-3aN"/>
                                </connections>
                            </button>
                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="GaP-be-PgI">
                                <rect key="frame" x="460" y="269" width="120" height="45"/>
                                <animations/>
                                <color key="backgroundColor" red="0.0" green="0.50196081400000003" blue="0.50196081400000003" alpha="1" colorSpace="calibratedRGB"/>
                                <constraints>
                                    <constraint firstAttribute="height" constant="45" id="F3U-L8-1UW"/>
                                    <constraint firstAttribute="width" constant="120" id="dt7-qT-cVm"/>
                                </constraints>
                                <color key="tintColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
                                <state key="normal" title="Sign"/>
                                <connections>
                                    <action selector="signText:" destination="BYZ-38-t0r" eventType="touchUpInside" id="h4t-VU-93F"/>
                                </connections>
                            </button>
                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="lSI-c1-j4r">
                                <rect key="frame" x="20" y="269" width="120" height="45"/>
                                <animations/>
                                <color key="backgroundColor" red="0.25098040700000002" green="0.50196081400000003" blue="0.0" alpha="1" colorSpace="calibratedRGB"/>
                                <constraints>
                                    <constraint firstAttribute="height" constant="45" id="8qh-kn-KUz"/>
                                    <constraint firstAttribute="width" constant="120" id="awd-fL-fRA"/>
                                </constraints>
                                <color key="tintColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
                                <state key="normal" title="Cypher"/>
                                <connections>
                                    <action selector="cypherText:" destination="BYZ-38-t0r" eventType="touchUpInside" id="nHc-hO-DWC"/>
                                </connections>
                            </button>
                        </subviews>
                        <animations/>
                        <color key="backgroundColor" white="1" alpha="1" colorSpace="custom" customColorSpace="calibratedWhite"/>
                        <constraints>
                            <constraint firstItem="Hxw-sy-EcD" firstAttribute="centerX" secondItem="22w-oY-3kk" secondAttribute="centerX" id="0Gf-qM-K1W"/>
                            <constraint firstItem="TCy-Eu-9P5" firstAttribute="centerX" secondItem="8bC-Xf-vdC" secondAttribute="centerX" id="3Vb-Mb-4Oo"/>
                            <constraint firstItem="TCy-Eu-9P5" firstAttribute="leading" secondItem="8bC-Xf-vdC" secondAttribute="leadingMargin" id="6PR-ZJ-zaW"/>
                            <constraint firstItem="kla-S3-7i3" firstAttribute="trailing" secondItem="TCy-Eu-9P5" secondAttribute="trailing" id="6gZ-h0-CI1"/>
                            <constraint firstItem="GaP-be-PgI" firstAttribute="trailing" secondItem="kkT-sX-2Lu" secondAttribute="trailing" id="740-Tg-dBa"/>
                            <constraint firstItem="f1A-A8-4kJ" firstAttribute="leading" secondItem="8bC-Xf-vdC" secondAttribute="leading" id="7dp-LN-IaQ"/>
                            <constraint firstItem="Hxw-sy-EcD" firstAttribute="top" secondItem="22w-oY-3kk" secondAttribute="bottom" constant="8" id="8I4-gT-oyf"/>
                            <constraint firstItem="TCy-Eu-9P5" firstAttribute="trailing" secondItem="8bC-Xf-vdC" secondAttribute="trailingMargin" id="BFb-xl-sUg"/>
                            <constraint firstItem="kkT-sX-2Lu" firstAttribute="centerX" secondItem="8bC-Xf-vdC" secondAttribute="centerX" id="BKS-Za-Ghd"/>
                            <constraint firstItem="f1A-A8-4kJ" firstAttribute="top" secondItem="8bC-Xf-vdC" secondAttribute="top" id="Br1-9z-mvH"/>
                            <constraint firstItem="22w-oY-3kk" firstAttribute="top" secondItem="7Oc-gW-REn" secondAttribute="bottom" constant="24" id="FN6-rB-F66"/>
                            <constraint firstItem="TCy-Eu-9P5" firstAttribute="top" secondItem="mvS-yU-sUC" secondAttribute="bottom" constant="8" id="Ipr-vY-bRn"/>
                            <constraint firstAttribute="trailing" secondItem="f1A-A8-4kJ" secondAttribute="trailing" id="JeR-eV-TT3"/>
                            <constraint firstItem="wfy-db-euE" firstAttribute="top" secondItem="f1A-A8-4kJ" secondAttribute="bottom" id="KYG-bM-h9g"/>
                            <constraint firstItem="GaP-be-PgI" firstAttribute="top" secondItem="kkT-sX-2Lu" secondAttribute="bottom" constant="8" id="LGK-fb-czh"/>
                            <constraint firstItem="mvS-yU-sUC" firstAttribute="top" secondItem="lSI-c1-j4r" secondAttribute="bottom" constant="22" id="OAa-eU-v7h"/>
                            <constraint firstItem="kla-S3-7i3" firstAttribute="top" secondItem="TCy-Eu-9P5" secondAttribute="bottom" constant="8" id="Q9d-y4-Xe9"/>
                            <constraint firstItem="7Oc-gW-REn" firstAttribute="centerX" secondItem="8bC-Xf-vdC" secondAttribute="centerX" id="R2f-QK-o0f"/>
                            <constraint firstItem="kkT-sX-2Lu" firstAttribute="leading" secondItem="8bC-Xf-vdC" secondAttribute="leadingMargin" id="RlV-XT-pCd"/>
                            <constraint firstItem="kkT-sX-2Lu" firstAttribute="top" secondItem="c1D-lJ-lUT" secondAttribute="bottom" constant="8" id="VIz-lo-6qo"/>
                            <constraint firstItem="22w-oY-3kk" firstAttribute="centerX" secondItem="8bC-Xf-vdC" secondAttribute="centerX" id="XPN-gb-q9H"/>
                            <constraint firstItem="lSI-c1-j4r" firstAttribute="top" secondItem="kkT-sX-2Lu" secondAttribute="bottom" constant="8" id="elK-nE-MH2"/>
                            <constraint firstItem="kkT-sX-2Lu" firstAttribute="trailing" secondItem="8bC-Xf-vdC" secondAttribute="trailingMargin" id="lw9-0r-W8w"/>
                            <constraint firstItem="c1D-lJ-lUT" firstAttribute="centerX" secondItem="8bC-Xf-vdC" secondAttribute="centerX" id="nty-0l-qpP"/>
                            <constraint firstItem="r36-YD-WXp" firstAttribute="top" secondItem="TCy-Eu-9P5" secondAttribute="bottom" constant="8" id="qZe-tr-ziL"/>
                            <constraint firstItem="7Oc-gW-REn" firstAttribute="top" secondItem="y3c-jy-aDJ" secondAttribute="bottom" constant="8" id="qvz-Js-gai"/>
                            <constraint firstItem="mvS-yU-sUC" firstAttribute="centerX" secondItem="8bC-Xf-vdC" secondAttribute="centerX" id="rea-q3-3hy"/>
                            <constraint firstItem="c1D-lJ-lUT" firstAttribute="top" secondItem="Hxw-sy-EcD" secondAttribute="bottom" constant="40" id="u44-cJ-NQP"/>
                            <constraint firstItem="lSI-c1-j4r" firstAttribute="leading" secondItem="kkT-sX-2Lu" secondAttribute="leading" id="u8e-ko-27W"/>
                            <constraint firstItem="r36-YD-WXp" firstAttribute="leading" secondItem="TCy-Eu-9P5" secondAttribute="leading" id="wLb-IY-EY5"/>
                        </constraints>
                    </view>
                    <connections>
                        <outlet property="clearTextTextfield" destination="kkT-sX-2Lu" id="hQz-B8-HeL"/>
                        <outlet property="cypherButton" destination="lSI-c1-j4r" id="A0G-FH-IS0"/>
                        <outlet property="cypheredTextTextfield" destination="TCy-Eu-9P5" id="6BJ-Ly-R7q"/>
                        <outlet property="decypherButton" destination="r36-YD-WXp" id="FLw-tf-UU0"/>
                        <outlet property="keyPairButton" destination="Hxw-sy-EcD" id="EfB-eC-iVo"/>
                        <outlet property="keyPairLabel" destination="22w-oY-3kk" id="Cc6-SA-XpX"/>
                        <outlet property="signButton" destination="GaP-be-PgI" id="dN2-R2-6qc"/>
                        <outlet property="verifySignatureButton" destination="kla-S3-7i3" id="3ch-qk-laU"/>
                    </connections>
                </viewController>
                <placeholder placeholderIdentifier="IBFirstResponder" id="dkx-z0-nzr" sceneMemberID="firstResponder"/>
            </objects>
            <point key="canvasLocation" x="913" y="657"/>
        </scene>
    </scenes>
    <resources>
        <image name="background" width="4288" height="2848"/>
    </resources>
</document>



================================================
FILE: AsymmetricCrypto.xcodeproj/project.pbxproj
================================================
// !$*UTF8*$!
{
	archiveVersion = 1;
	classes = {
	};
	objectVersion = 46;
	objects = {

/* Begin PBXBuildFile section */
		66D4870E1BC114CA009F2E52 /* AppDelegate.swift in Sources */ = {isa = PBXBuildFile; fileRef = 66D4870D1BC114CA009F2E52 /* AppDelegate.swift */; };
		66D487101BC114CA009F2E52 /* ViewController.swift in Sources */ = {isa = PBXBuildFile; fileRef = 66D4870F1BC114CA009F2E52 /* ViewController.swift */; };
		66D487131BC114CA009F2E52 /* Main.storyboard in Resources */ = {isa = PBXBuildFile; fileRef = 66D487111BC114CA009F2E52 /* Main.storyboard */; };
		66D487151BC114CB009F2E52 /* Assets.xcassets in Resources */ = {isa = PBXBuildFile; fileRef = 66D487141BC114CB009F2E52 /* Assets.xcassets */; };
		66D487181BC114CB009F2E52 /* LaunchScreen.storyboard in Resources */ = {isa = PBXBuildFile; fileRef = 66D487161BC114CB009F2E52 /* LaunchScreen.storyboard */; };
		66D487201BC11518009F2E52 /* AsymmetricCryptoManager.swift in Sources */ = {isa = PBXBuildFile; fileRef = 66D4871F1BC11518009F2E52 /* AsymmetricCryptoManager.swift */; };
		66D487251BC12828009F2E52 /* UIViewController+Alerts.swift in Sources */ = {isa = PBXBuildFile; fileRef = 66D487241BC12828009F2E52 /* UIViewController+Alerts.swift */; };
/* End PBXBuildFile section */

/* Begin PBXFileReference section */
		661EE2F11DAA9D6500A8BEFB /* AsymmetricCrypto.entitlements */ = {isa = PBXFileReference; lastKnownFileType = text.plist.entitlements; path = AsymmetricCrypto.entitlements; sourceTree = "<group>"; };
		66D4870A1BC114CA009F2E52 /* AsymmetricCrypto.app */ = {isa = PBXFileReference; explicitFileType = wrapper.application; includeInIndex = 0; path = AsymmetricCrypto.app; sourceTree = BUILT_PRODUCTS_DIR; };
		66D4870D1BC114CA009F2E52 /* AppDelegate.swift */ = {isa = PBXFileReference; lastKnownFileType = sourcecode.swift; path = AppDelegate.swift; sourceTree = "<group>"; };
		66D4870F1BC114CA009F2E52 /* ViewController.swift */ = {isa = PBXFileReference; lastKnownFileType = sourcecode.swift; path = ViewController.swift; sourceTree = "<group>"; };
		66D487121BC114CA009F2E52 /* Base */ = {isa = PBXFileReference; lastKnownFileType = file.storyboard; name = Base; path = Base.lproj/Main.storyboard; sourceTree = "<group>"; };
		66D487141BC114CB009F2E52 /* Assets.xcassets */ = {isa = PBXFileReference; lastKnownFileType = folder.assetcatalog; path = Assets.xcassets; sourceTree = "<group>"; };
		66D487171BC114CB009F2E52 /* Base */ = {isa = PBXFileReference; lastKnownFileType = file.storyboard; name = Base; path = Base.lproj/LaunchScreen.storyboard; sourceTree = "<group>"; };
		66D487191BC114CB009F2E52 /* Info.plist */ = {isa = PBXFileReference; lastKnownFileType = text.plist.xml; path = Info.plist; sourceTree = "<group>"; };
		66D4871F1BC11518009F2E52 /* AsymmetricCryptoManager.swift */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.swift; path = AsymmetricCryptoManager.swift; sourceTree = "<group>"; };
		66D487211BC121A0009F2E52 /* AsymmetricCrypto-Bridging-Header.h */ = {isa = PBXFileReference; lastKnownFileType = sourcecode.c.h; path = "AsymmetricCrypto-Bridging-Header.h"; sourceTree = "<group>"; };
		66D487241BC12828009F2E52 /* UIViewController+Alerts.swift */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.swift; path = "UIViewController+Alerts.swift"; sourceTree = "<group>"; };
/* End PBXFileReference section */

/* Begin PBXFrameworksBuildPhase section */
		66D487071BC114CA009F2E52 /* Frameworks */ = {
			isa = PBXFrameworksBuildPhase;
			buildActionMask = 2147483647;
			files = (
			);
			runOnlyForDeploymentPostprocessing = 0;
		};
/* End PBXFrameworksBuildPhase section */

/* Begin PBXGroup section */
		66D487011BC114CA009F2E52 = {
			isa = PBXGroup;
			children = (
				66D4870C1BC114CA009F2E52 /* AsymmetricCrypto */,
				66D4870B1BC114CA009F2E52 /* Products */,
			);
			sourceTree = "<group>";
		};
		66D4870B1BC114CA009F2E52 /* Products */ = {
			isa = PBXGroup;
			children = (
				66D4870A1BC114CA009F2E52 /* AsymmetricCrypto.app */,
			);
			name = Products;
			sourceTree = "<group>";
		};
		66D4870C1BC114CA009F2E52 /* AsymmetricCrypto */ = {
			isa = PBXGroup;
			children = (
				661EE2F11DAA9D6500A8BEFB /* AsymmetricCrypto.entitlements */,
				66D4870D1BC114CA009F2E52 /* AppDelegate.swift */,
				66D487241BC12828009F2E52 /* UIViewController+Alerts.swift */,
				66D4870F1BC114CA009F2E52 /* ViewController.swift */,
				66D487111BC114CA009F2E52 /* Main.storyboard */,
				66D487141BC114CB009F2E52 /* Assets.xcassets */,
				66D487161BC114CB009F2E52 /* LaunchScreen.storyboard */,
				66D487191BC114CB009F2E52 /* Info.plist */,
				66D4871F1BC11518009F2E52 /* AsymmetricCryptoManager.swift */,
				66D487211BC121A0009F2E52 /* AsymmetricCrypto-Bridging-Header.h */,
			);
			path = AsymmetricCrypto;
			sourceTree = "<group>";
		};
/* End PBXGroup section */

/* Begin PBXNativeTarget section */
		66D487091BC114CA009F2E52 /* AsymmetricCrypto */ = {
			isa = PBXNativeTarget;
			buildConfigurationList = 66D4871C1BC114CB009F2E52 /* Build configuration list for PBXNativeTarget "AsymmetricCrypto" */;
			buildPhases = (
				66D487061BC114CA009F2E52 /* Sources */,
				66D487071BC114CA009F2E52 /* Frameworks */,
				66D487081BC114CA009F2E52 /* Resources */,
			);
			buildRules = (
			);
			dependencies = (
			);
			name = AsymmetricCrypto;
			productName = AsymmetricCrypto;
			productReference = 66D4870A1BC114CA009F2E52 /* AsymmetricCrypto.app */;
			productType = "com.apple.product-type.application";
		};
/* End PBXNativeTarget section */

/* Begin PBXProject section */
		66D487021BC114CA009F2E52 /* Project object */ = {
			isa = PBXProject;
			attributes = {
				LastSwiftUpdateCheck = 0700;
				LastUpgradeCheck = 0800;
				ORGANIZATIONNAME = "Ignacio Nieto Carvajal";
				TargetAttributes = {
					66D487091BC114CA009F2E52 = {
						CreatedOnToolsVersion = 7.0.1;
						DevelopmentTeam = 97P9DZHP78;
						LastSwiftMigration = 0800;
						SystemCapabilities = {
							com.apple.Keychain = {
								enabled = 1;
							};
						};
					};
				};
			};
			buildConfigurationList = 66D487051BC114CA009F2E52 /* Build configuration list for PBXProject "AsymmetricCrypto" */;
			compatibilityVersion = "Xcode 3.2";
			developmentRegion = English;
			hasScannedForEncodings = 0;
			knownRegions = (
				en,
				Base,
			);
			mainGroup = 66D487011BC114CA009F2E52;
			productRefGroup = 66D4870B1BC114CA009F2E52 /* Products */;
			projectDirPath = "";
			projectRoot = "";
			targets = (
				66D487091BC114CA009F2E52 /* AsymmetricCrypto */,
			);
		};
/* End PBXProject section */

/* Begin PBXResourcesBuildPhase section */
		66D487081BC114CA009F2E52 /* Resources */ = {
			isa = PBXResourcesBuildPhase;
			buildActionMask = 2147483647;
			files = (
				66D487181BC114CB009F2E52 /* LaunchScreen.storyboard in Resources */,
				66D487151BC114CB009F2E52 /* Assets.xcassets in Resources */,
				66D487131BC114CA009F2E52 /* Main.storyboard in Resources */,
			);
			runOnlyForDeploymentPostprocessing = 0;
		};
/* End PBXResourcesBuildPhase section */

/* Begin PBXSourcesBuildPhase section */
		66D487061BC114CA009F2E52 /* Sources */ = {
			isa = PBXSourcesBuildPhase;
			buildActionMask = 2147483647;
			files = (
				66D487101BC114CA009F2E52 /* ViewController.swift in Sources */,
				66D4870E1BC114CA009F2E52 /* AppDelegate.swift in Sources */,
				66D487201BC11518009F2E52 /* AsymmetricCryptoManager.swift in Sources */,
				66D487251BC12828009F2E52 /* UIViewController+Alerts.swift in Sources */,
			);
			runOnlyForDeploymentPostprocessing = 0;
		};
/* End PBXSourcesBuildPhase section */

/* Begin PBXVariantGroup section */
		66D487111BC114CA009F2E52 /* Main.storyboard */ = {
			isa = PBXVariantGroup;
			children = (
				66D487121BC114CA009F2E52 /* Base */,
			);
			name = Main.storyboard;
			sourceTree = "<group>";
		};
		66D487161BC114CB009F2E52 /* LaunchScreen.storyboard */ = {
			isa = PBXVariantGroup;
			children = (
				66D487171BC114CB009F2E52 /* Base */,
			);
			name = LaunchScreen.storyboard;
			sourceTree = "<group>";
		};
/* End PBXVariantGroup section */

/* Begin XCBuildConfiguration section */
		66D4871A1BC114CB009F2E52 /* Debug */ = {
			isa = XCBuildConfiguration;
			buildSettings = {
				ALWAYS_SEARCH_USER_PATHS = NO;
				CLANG_CXX_LANGUAGE_STANDARD = "gnu++0x";
				CLANG_CXX_LIBRARY = "libc++";
				CLANG_ENABLE_MODULES = YES;
				CLANG_ENABLE_OBJC_ARC = YES;
				CLANG_WARN_BOOL_CONVERSION = YES;
				CLANG_WARN_CONSTANT_CONVERSION = YES;
				CLANG_WARN_DIRECT_OBJC_ISA_USAGE = YES_ERROR;
				CLANG_WARN_EMPTY_BODY = YES;
				CLANG_WARN_ENUM_CONVERSION = YES;
				CLANG_WARN_INFINITE_RECURSION = YES;
				CLANG_WARN_INT_CONVERSION = YES;
				CLANG_WARN_OBJC_ROOT_CLASS = YES_ERROR;
				CLANG_WARN_SUSPICIOUS_MOVE = YES;
				CLANG_WARN_UNREACHABLE_CODE = YES;
				CLANG_WARN__DUPLICATE_METHOD_MATCH = YES;
				"CODE_SIGN_IDENTITY[sdk=iphoneos*]" = "iPhone Developer";
				COPY_PHASE_STRIP = NO;
				DEBUG_INFORMATION_FORMAT = dwarf;
				ENABLE_STRICT_OBJC_MSGSEND = YES;
				ENABLE_TESTABILITY = YES;
				GCC_C_LANGUAGE_STANDARD = gnu99;
				GCC_DYNAMIC_NO_PIC = NO;
				GCC_NO_COMMON_BLOCKS = YES;
				GCC_OPTIMIZATION_LEVEL = 0;
				GCC_PREPROCESSOR_DEFINITIONS = (
					"DEBUG=1",
					"$(inherited)",
				);
				GCC_WARN_64_TO_32_BIT_CONVERSION = YES;
				GCC_WARN_ABOUT_RETURN_TYPE = YES_ERROR;
				GCC_WARN_UNDECLARED_SELECTOR = YES;
				GCC_WARN_UNINITIALIZED_AUTOS = YES_AGGRESSIVE;
				GCC_WARN_UNUSED_FUNCTION = YES;
				GCC_WARN_UNUSED_VARIABLE = YES;
				IPHONEOS_DEPLOYMENT_TARGET = 9.0;
				MTL_ENABLE_DEBUG_INFO = YES;
				ONLY_ACTIVE_ARCH = YES;
				SDKROOT = iphoneos;
				SWIFT_OPTIMIZATION_LEVEL = "-Onone";
			};
			name = Debug;
		};
		66D4871B1BC114CB009F2E52 /* Release */ = {
			isa = XCBuildConfiguration;
			buildSettings = {
				ALWAYS_SEARCH_USER_PATHS = NO;
				CLANG_CXX_LANGUAGE_STANDARD = "gnu++0x";
				CLANG_CXX_LIBRARY = "libc++";
				CLANG_ENABLE_MODULES = YES;
				CLANG_ENABLE_OBJC_ARC = YES;
				CLANG_WARN_BOOL_CONVERSION = YES;
				CLANG_WARN_CONSTANT_CONVERSION = YES;
				CLANG_WARN_DIRECT_OBJC_ISA_USAGE = YES_ERROR;
				CLANG_WARN_EMPTY_BODY = YES;
				CLANG_WARN_ENUM_CONVERSION = YES;
				CLANG_WARN_INFINITE_RECURSION = YES;
				CLANG_WARN_INT_CONVERSION = YES;
				CLANG_WARN_OBJC_ROOT_CLASS = YES_ERROR;
				CLANG_WARN_SUSPICIOUS_MOVE = YES;
				CLANG_WARN_UNREACHABLE_CODE = YES;
				CLANG_WARN__DUPLICATE_METHOD_MATCH = YES;
				"CODE_SIGN_IDENTITY[sdk=iphoneos*]" = "iPhone Developer";
				COPY_PHASE_STRIP = NO;
				DEBUG_INFORMATION_FORMAT = "dwarf-with-dsym";
				ENABLE_NS_ASSERTIONS = NO;
				ENABLE_STRICT_OBJC_MSGSEND = YES;
				GCC_C_LANGUAGE_STANDARD = gnu99;
				GCC_NO_COMMON_BLOCKS = YES;
				GCC_WARN_64_TO_32_BIT_CONVERSION = YES;
				GCC_WARN_ABOUT_RETURN_TYPE = YES_ERROR;
				GCC_WARN_UNDECLARED_SELECTOR = YES;
				GCC_WARN_UNINITIALIZED_AUTOS = YES_AGGRESSIVE;
				GCC_WARN_UNUSED_FUNCTION = YES;
				GCC_WARN_UNUSED_VARIABLE = YES;
				IPHONEOS_DEPLOYMENT_TARGET = 9.0;
				MTL_ENABLE_DEBUG_INFO = NO;
				SDKROOT = iphoneos;
				SWIFT_OPTIMIZATION_LEVEL = "-Owholemodule";
				VALIDATE_PRODUCT = YES;
			};
			name = Release;
		};
		66D4871D1BC114CB009F2E52 /* Debug */ = {
			isa = XCBuildConfiguration;
			buildSettings = {
				ASSETCATALOG_COMPILER_APPICON_NAME = AppIcon;
				CLANG_ENABLE_MODULES = YES;
				CODE_SIGN_ENTITLEMENTS = AsymmetricCrypto/AsymmetricCrypto.entitlements;
				DEVELOPMENT_TEAM = 97P9DZHP78;
				INFOPLIST_FILE = AsymmetricCrypto/Info.plist;
				LD_RUNPATH_SEARCH_PATHS = "$(inherited) @executable_path/Frameworks";
				PRODUCT_BUNDLE_IDENTIFIER = "com.Ignacio-Nieto-Carvajal.AsymmetricCrypto";
				PRODUCT_NAME = "$(TARGET_NAME)";
				SWIFT_OBJC_BRIDGING_HEADER = "AsymmetricCrypto/AsymmetricCrypto-Bridging-Header.h";
				SWIFT_OPTIMIZATION_LEVEL = "-Onone";
				SWIFT_VERSION = 3.0;
			};
			name = Debug;
		};
		66D4871E1BC114CB009F2E52 /* Release */ = {
			isa = XCBuildConfiguration;
			buildSettings = {
				ASSETCATALOG_COMPILER_APPICON_NAME = AppIcon;
				CLANG_ENABLE_MODULES = YES;
				CODE_SIGN_ENTITLEMENTS = AsymmetricCrypto/AsymmetricCrypto.entitlements;
				DEVELOPMENT_TEAM = 97P9DZHP78;
				INFOPLIST_FILE = AsymmetricCrypto/Info.plist;
				LD_RUNPATH_SEARCH_PATHS = "$(inherited) @executable_path/Frameworks";
				PRODUCT_BUNDLE_IDENTIFIER = "com.Ignacio-Nieto-Carvajal.AsymmetricCrypto";
				PRODUCT_NAME = "$(TARGET_NAME)";
				SWIFT_OBJC_BRIDGING_HEADER = "AsymmetricCrypto/AsymmetricCrypto-Bridging-Header.h";
				SWIFT_VERSION = 3.0;
			};
			name = Release;
		};
/* End XCBuildConfiguration section */

/* Begin XCConfigurationList section */
		66D487051BC114CA009F2E52 /* Build configuration list for PBXProject "AsymmetricCrypto" */ = {
			isa = XCConfigurationList;
			buildConfigurations = (
				66D4871A1BC114CB009F2E52 /* Debug */,
				66D4871B1BC114CB009F2E52 /* Release */,
			);
			defaultConfigurationIsVisible = 0;
			defaultConfigurationName = Release;
		};
		66D4871C1BC114CB009F2E52 /* Build configuration list for PBXNativeTarget "AsymmetricCrypto" */ = {
			isa = XCConfigurationList;
			buildConfigurations = (
				66D4871D1BC114CB009F2E52 /* Debug */,
				66D4871E1BC114CB009F2E52 /* Release */,
			);
			defaultConfigurationIsVisible = 0;
			defaultConfigurationName = Release;
		};
/* End XCConfigurationList section */
	};
	rootObject = 66D487021BC114CA009F2E52 /* Project object */;
}



================================================
FILE: AsymmetricCrypto.xcodeproj/project.xcworkspace/contents.xcworkspacedata
================================================
<?xml version="1.0" encoding="UTF-8"?>
<Workspace
   version = "1.0">
   <FileRef
      location = "self:AsymmetricCrypto.xcodeproj">
   </FileRef>
</Workspace>



================================================
FILE: AsymmetricCrypto.xcodeproj/xcuserdata/Nacho.xcuserdatad/xcdebugger/Breakpoints_v2.xcbkptlist
================================================
<?xml version="1.0" encoding="UTF-8"?>
<Bucket
   type = "1"
   version = "2.0">
   <Breakpoints>
      <BreakpointProxy
         BreakpointExtensionID = "Xcode.Breakpoint.FileBreakpoint">
         <BreakpointContent
            shouldBeEnabled = "No"
            ignoreCount = "0"
            continueAfterRunningActions = "No"
            filePath = "AsymmetricCrypto/AsymmetricCryptoManager.swift"
            timestampString = "502919477.729367"
            startingColumnNumber = "9223372036854775807"
            endingColumnNumber = "9223372036854775807"
            startingLineNumber = "166"
            endingLineNumber = "166"
            landmarkName = "encryptMessageWithPublicKey(_:completion:)"
            landmarkType = "7">
         </BreakpointContent>
      </BreakpointProxy>
   </Breakpoints>
</Bucket>



================================================
FILE: AsymmetricCrypto.xcodeproj/xcuserdata/Nacho.xcuserdatad/xcschemes/AsymmetricCrypto.xcscheme
================================================
<?xml version="1.0" encoding="UTF-8"?>
<Scheme
   LastUpgradeVersion = "0800"
   version = "1.3">
   <BuildAction
      parallelizeBuildables = "YES"
      buildImplicitDependencies = "YES">
      <BuildActionEntries>
         <BuildActionEntry
            buildForTesting = "YES"
            buildForRunning = "YES"
            buildForProfiling = "YES"
            buildForArchiving = "YES"
            buildForAnalyzing = "YES">
            <BuildableReference
               BuildableIdentifier = "primary"
               BlueprintIdentifier = "66D487091BC114CA009F2E52"
               BuildableName = "AsymmetricCrypto.app"
               BlueprintName = "AsymmetricCrypto"
               ReferencedContainer = "container:AsymmetricCrypto.xcodeproj">
            </BuildableReference>
         </BuildActionEntry>
      </BuildActionEntries>
   </BuildAction>
   <TestAction
      buildConfiguration = "Debug"
      selectedDebuggerIdentifier = "Xcode.DebuggerFoundation.Debugger.LLDB"
      selectedLauncherIdentifier = "Xcode.DebuggerFoundation.Launcher.LLDB"
      shouldUseLaunchSchemeArgsEnv = "YES">
      <Testables>
      </Testables>
      <MacroExpansion>
         <BuildableReference
            BuildableIdentifier = "primary"
            BlueprintIdentifier = "66D487091BC114CA009F2E52"
            BuildableName = "AsymmetricCrypto.app"
            BlueprintName = "AsymmetricCrypto"
            ReferencedContainer = "container:AsymmetricCrypto.xcodeproj">
         </BuildableReference>
      </MacroExpansion>
      <AdditionalOptions>
      </AdditionalOptions>
   </TestAction>
   <LaunchAction
      buildConfiguration = "Debug"
      selectedDebuggerIdentifier = "Xcode.DebuggerFoundation.Debugger.LLDB"
      selectedLauncherIdentifier = "Xcode.DebuggerFoundation.Launcher.LLDB"
      launchStyle = "0"
      useCustomWorkingDirectory = "NO"
      ignoresPersistentStateOnLaunch = "NO"
      debugDocumentVersioning = "YES"
      debugServiceExtension = "internal"
      allowLocationSimulation = "YES">
      <BuildableProductRunnable
         runnableDebuggingMode = "0">
         <BuildableReference
            BuildableIdentifier = "primary"
            BlueprintIdentifier = "66D487091BC114CA009F2E52"
            BuildableName = "AsymmetricCrypto.app"
            BlueprintName = "AsymmetricCrypto"
            ReferencedContainer = "container:AsymmetricCrypto.xcodeproj">
         </BuildableReference>
      </BuildableProductRunnable>
      <AdditionalOptions>
      </AdditionalOptions>
   </LaunchAction>
   <ProfileAction
      buildConfiguration = "Release"
      shouldUseLaunchSchemeArgsEnv = "YES"
      savedToolIdentifier = ""
      useCustomWorkingDirectory = "NO"
      debugDocumentVersioning = "YES">
      <BuildableProductRunnable
         runnableDebuggingMode = "0">
         <BuildableReference
            BuildableIdentifier = "primary"
            BlueprintIdentifier = "66D487091BC114CA009F2E52"
            BuildableName = "AsymmetricCrypto.app"
            BlueprintName = "AsymmetricCrypto"
            ReferencedContainer = "container:AsymmetricCrypto.xcodeproj">
         </BuildableReference>
      </BuildableProductRunnable>
   </ProfileAction>
   <AnalyzeAction
      buildConfiguration = "Debug">
   </AnalyzeAction>
   <ArchiveAction
      buildConfiguration = "Release"
      revealArchiveInOrganizer = "YES">
   </ArchiveAction>
</Scheme>



================================================
FILE: AsymmetricCrypto.xcodeproj/xcuserdata/Nacho.xcuserdatad/xcschemes/xcschememanagement.plist
================================================
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>SchemeUserState</key>
	<dict>
		<key>AsymmetricCrypto.xcscheme</key>
		<dict>
			<key>orderHint</key>
			<integer>0</integer>
		</dict>
	</dict>
	<key>SuppressBuildableAutocreation</key>
	<dict>
		<key>66D487091BC114CA009F2E52</key>
		<dict>
			<key>primary</key>
			<true/>
		</dict>
	</dict>
</dict>
</plist>


